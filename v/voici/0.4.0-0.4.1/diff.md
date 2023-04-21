# Comparing `tmp/voici-0.4.0.tar.gz` & `tmp/voici-0.4.1.tar.gz`

## Comparing `voici-0.4.0.tar` & `voici-0.4.1.tar`

### file list

```diff
@@ -1,188 +1,189 @@
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 voici-0.4.0/.eslintignore
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 voici-0.4.0/.eslintrc.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 voici-0.4.0/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 voici-0.4.0/.prettierrc
--rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 voici-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 voici-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 voici-0.4.0/RELEASE.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 voici-0.4.0/environment.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 voici-0.4.0/lerna.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 voici-0.4.0/lint-staged.config.js
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 voici-0.4.0/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 voici-0.4.0/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 voici-0.4.0/setup.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.0/tsconfig.eslint.json
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 voici-0.4.0/tsconfigbase.json
--rw-r--r--   0        0        0   537654 2020-02-02 00:00:00.000000 voici-0.4.0/yarn.lock
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.0/demo/environment.yml
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 voici-0.4.0/demo/notebooks/iris.csv
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 voici-0.4.0/demo/notebooks/voici.ipynb
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 voici-0.4.0/demo/notebooks/widgets/bqplot.ipynb
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 voici-0.4.0/demo/notebooks/widgets/ipycanvas.ipynb
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 voici-0.4.0/docs/changelog.md
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 voici-0.4.0/docs/conf.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 voici-0.4.0/docs/configuration.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 voici-0.4.0/docs/contributing.md
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 voici-0.4.0/docs/deploy.md
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 voici-0.4.0/docs/environment.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 voici-0.4.0/docs/index.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 voici-0.4.0/docs/install.md
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 voici-0.4.0/docs/voila-logo.svg
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 voici-0.4.0/scripts/bump-version.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/package.json
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png
--rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png
--rw-r--r--   0        0        0   186883 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png
--rw-r--r--   0        0        0    46536 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png
--rw-r--r--   0        0        0    53032 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png
--rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png
--rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png
--rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png
--rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 voici-0.4.0/voici/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 voici-0.4.0/voici/__main__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 voici-0.4.0/voici/_version.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 voici-0.4.0/voici/addon.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 voici-0.4.0/voici/app.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 voici-0.4.0/voici/exporter.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 voici-0.4.0/voici/tree_exporter.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/index.html
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1023.js
--rw-r--r--   0        0        0   599879 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1024.js
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/103.js
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1053.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1058.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1100.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1105.js
--rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1432.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1497.js
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1553.js
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1581.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1667.js
--rw-r--r--   0        0        0    53409 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1672.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1672.js.LICENSE.txt
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1732.js
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1770.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1890.js
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1980.js
--rw-r--r--   0        0        0    24245 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2075.js
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2106.js
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2230.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2266.js
--rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2322.js
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2359.js
--rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2361.js
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2488.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2516.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2630.js
--rw-r--r--   0        0        0    11565 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2687.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/275.js
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2784.js
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2784.js.LICENSE.txt
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/286.js
--rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2950.js
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3008.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3086.js
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3251.js
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3256.js
--rw-r--r--   0        0        0   432937 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/330.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3305.js
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3312.js
--rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3316.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3316.js.LICENSE.txt
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3349.js
--rw-r--r--   0        0        0   198935 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/339.js
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3504.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3655.js
--rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3693.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3811.js
--rw-r--r--   0        0        0   152146 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3851.js
--rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3922.js
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4259.js
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4359.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4382.js
--rw-r--r--   0        0        0   173449 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/450.js
--rw-r--r--   0        0        0    44048 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4530.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4530.js.LICENSE.txt
--rw-r--r--   0        0        0    33749 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4875.js
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4896.js
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4939.js
--rw-r--r--   0        0        0   901507 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4963.js
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4963.js.LICENSE.txt
--rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4977.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5188.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5291.js
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/53.js
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5403.js
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5445.js
--rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5474.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5826.js
--rw-r--r--   0        0        0   103087 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5950.js
--rw-r--r--   0        0        0   306356 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5952.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5952.js.LICENSE.txt
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/596.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5985.js
--rw-r--r--   0        0        0    31585 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6111.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6178.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6196.js
--rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6219.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6219.js.LICENSE.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6417.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6527.js
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6587.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6614.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6616.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6757.js
--rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6770.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6790.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6839.js
--rw-r--r--   0        0        0    10288 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6852.js
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6856.js
--rw-r--r--   0        0        0    88422 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6914.js
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6976.js
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7003.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7015.js
--rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7066.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/709.js
--rw-r--r--   0        0        0    89502 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/74.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7469.js
--rw-r--r--   0        0        0    82106 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7560.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7623.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7695.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7795.js
--rw-r--r--   0        0        0    37531 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8085.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8164.js
--rw-r--r--   0        0        0    89999 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8291.js
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8291.js.LICENSE.txt
--rw-r--r--   0        0        0   123750 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8316.js
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8316.js.LICENSE.txt
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/846.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/86.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8679.js
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8809.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8874.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9060.js
--rw-r--r--   0        0        0   528943 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9112.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9320.js
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9339.js
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9406.js
--rw-r--r--   0        0        0   135493 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9513.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9513.js.LICENSE.txt
--rw-r--r--   0        0        0   248014 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9727.js
--rw-r--r--   0        0        0    53651 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9757.js
--rw-r--r--   0        0        0    37027 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9780.js
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9807.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9817.js
--rw-r--r--   0        0        0    84485 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9900.js
--rw-r--r--   0        0        0    22979 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9988.js
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/service-worker-b2fb40a.js
--rw-r--r--   0        0        0    23293 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/treepage.js
--rw-r--r--   0        0        0    24001 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/voici.js
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 voici-0.4.0/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 voici-0.4.0/LICENSE
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 voici-0.4.0/README.md
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 voici-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 voici-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 voici-0.4.1/.eslintignore
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 voici-0.4.1/.eslintrc.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 voici-0.4.1/.prettierignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 voici-0.4.1/.prettierrc
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 voici-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 voici-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 voici-0.4.1/RELEASE.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 voici-0.4.1/environment.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 voici-0.4.1/lerna.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 voici-0.4.1/lint-staged.config.js
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 voici-0.4.1/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 voici-0.4.1/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 voici-0.4.1/setup.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 voici-0.4.1/tsconfigbase.json
+-rw-r--r--   0        0        0   537654 2020-02-02 00:00:00.000000 voici-0.4.1/yarn.lock
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.1/demo/environment.yml
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 voici-0.4.1/demo/notebooks/iris.csv
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 voici-0.4.1/demo/notebooks/voici.ipynb
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 voici-0.4.1/demo/notebooks/widgets/bqplot.ipynb
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 voici-0.4.1/demo/notebooks/widgets/ipycanvas.ipynb
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 voici-0.4.1/docs/changelog.md
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 voici-0.4.1/docs/conf.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 voici-0.4.1/docs/configuration.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 voici-0.4.1/docs/contributing.md
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 voici-0.4.1/docs/deploy.md
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 voici-0.4.1/docs/environment.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 voici-0.4.1/docs/index.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 voici-0.4.1/docs/install.md
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 voici-0.4.1/docs/voila-logo.svg
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 voici-0.4.1/scripts/bump-version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/package.json
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png
+-rw-r--r--   0        0        0   186883 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png
+-rw-r--r--   0        0        0    46536 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png
+-rw-r--r--   0        0        0    53032 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png
+-rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png
+-rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png
+-rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 voici-0.4.1/voici/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 voici-0.4.1/voici/__main__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 voici-0.4.1/voici/_version.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 voici-0.4.1/voici/addon.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 voici-0.4.1/voici/app.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 voici-0.4.1/voici/exporter.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 voici-0.4.1/voici/tree_exporter.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/index.html
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1023.js
+-rw-r--r--   0        0        0   599879 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1024.js
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/103.js
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1053.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1058.js
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1100.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1105.js
+-rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1432.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1497.js
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1553.js
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1581.js
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1667.js
+-rw-r--r--   0        0        0    53409 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1672.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1672.js.LICENSE.txt
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1732.js
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1770.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1890.js
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/1980.js
+-rw-r--r--   0        0        0    24245 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2075.js
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2106.js
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2230.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2266.js
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2322.js
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2359.js
+-rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2361.js
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2488.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2516.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2630.js
+-rw-r--r--   0        0        0    11565 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2687.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/275.js
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2784.js
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2784.js.LICENSE.txt
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/286.js
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/2950.js
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3008.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3086.js
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3251.js
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3256.js
+-rw-r--r--   0        0        0   432937 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/330.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3305.js
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3312.js
+-rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3316.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3316.js.LICENSE.txt
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3349.js
+-rw-r--r--   0        0        0   198935 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/339.js
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3504.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3655.js
+-rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3693.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3811.js
+-rw-r--r--   0        0        0   152146 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3851.js
+-rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/3922.js
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4259.js
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4359.js
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4382.js
+-rw-r--r--   0        0        0   173449 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/450.js
+-rw-r--r--   0        0        0    44048 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4530.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4530.js.LICENSE.txt
+-rw-r--r--   0        0        0    33749 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4875.js
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4896.js
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4939.js
+-rw-r--r--   0        0        0   901522 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4963.js
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4963.js.LICENSE.txt
+-rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/4977.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5188.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5291.js
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/53.js
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5403.js
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5445.js
+-rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5474.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5826.js
+-rw-r--r--   0        0        0   104080 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5950.js
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5950.js.LICENSE.txt
+-rw-r--r--   0        0        0   306356 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5952.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5952.js.LICENSE.txt
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/596.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/5985.js
+-rw-r--r--   0        0        0    31585 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6111.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6178.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6196.js
+-rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6219.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6219.js.LICENSE.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6417.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6527.js
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6587.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6614.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6616.js
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6757.js
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6770.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6790.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6839.js
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6852.js
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6856.js
+-rw-r--r--   0        0        0    88422 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6914.js
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/6976.js
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7003.js
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7015.js
+-rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7066.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/709.js
+-rw-r--r--   0        0        0    89502 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/74.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7469.js
+-rw-r--r--   0        0        0    82106 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7560.js
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7623.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7695.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/7795.js
+-rw-r--r--   0        0        0    37531 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8085.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8164.js
+-rw-r--r--   0        0        0    89999 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8291.js
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8291.js.LICENSE.txt
+-rw-r--r--   0        0        0   123750 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8316.js
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8316.js.LICENSE.txt
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/846.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/86.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8679.js
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8809.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/8874.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9060.js
+-rw-r--r--   0        0        0   528943 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9112.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9320.js
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9339.js
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9406.js
+-rw-r--r--   0        0        0   135493 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9513.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9513.js.LICENSE.txt
+-rw-r--r--   0        0        0   248014 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9727.js
+-rw-r--r--   0        0        0    53651 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9757.js
+-rw-r--r--   0        0        0    37027 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9780.js
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9807.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9817.js
+-rw-r--r--   0        0        0    84485 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9900.js
+-rw-r--r--   0        0        0    22979 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/9988.js
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/service-worker-b2fb40a.js
+-rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/treepage.js
+-rw-r--r--   0        0        0    24220 2020-02-02 00:00:00.000000 voici-0.4.1/voici/static/build/voici.js
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 voici-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 voici-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 voici-0.4.1/README.md
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 voici-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 voici-0.4.1/PKG-INFO
```

### Comparing `voici-0.4.0/.eslintrc.js` & `voici-0.4.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/CHANGELOG.md` & `voici-0.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.4.1
+
+([Full Changelog](https://github.com/voila-dashboards/voici/compare/@voila-dashboards/voici@0.4.0...417746aff5b4f3faa7b254e8c516a46e59a67155))
+
+### Enhancements made
+
+- Add missing `react-dom` module to Webpack shared scope [#67](https://github.com/voila-dashboards/voici/pull/67) ([@trungleduc](https://github.com/trungleduc))
+
+### Maintenance and upkeep improvements
+
+- Remove old logic for installing piplite packages [#68](https://github.com/voila-dashboards/voici/pull/68) ([@martinRenou](https://github.com/martinRenou))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/voila-dashboards/voici/graphs/contributors?from=2023-04-18&to=2023-04-21&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Agithub-actions+updated%3A2023-04-18..2023-04-21&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3AmartinRenou+updated%3A2023-04-18..2023-04-21&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Atrungleduc+updated%3A2023-04-18..2023-04-21&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.4.0
 
 ([Full Changelog](https://github.com/voila-dashboards/voici/compare/v0.3.3...3fb43ef1d143a3e78939e7e35d293cda01d58867))
 
 ### Enhancements made
 
 - Update CLI [#65](https://github.com/voila-dashboards/voici/pull/65) ([@trungleduc](https://github.com/trungleduc))
@@ -17,16 +37,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/voila-dashboards/voici/graphs/contributors?from=2023-04-13&to=2023-04-18&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Agithub-actions+updated%3A2023-04-13..2023-04-18&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Ajtpio+updated%3A2023-04-13..2023-04-18&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3AmartinRenou+updated%3A2023-04-13..2023-04-18&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Atrungleduc+updated%3A2023-04-13..2023-04-18&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.3.3
 
 ([Full Changelog](https://github.com/voila-dashboards/voici/compare/@voila-dashboards/voici@0.3.2...1e5b08a398d89d69bcdd746ec47fb09be5b8f0df))
 
 ### Enhancements made
 
 - Fix handling of the base url to enable the Service Worker [#59](https://github.com/voila-dashboards/voici/pull/59) ([@jtpio](https://github.com/jtpio))
```

### Comparing `voici-0.4.0/CONTRIBUTING.md` & `voici-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/RELEASE.md` & `voici-0.4.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/lint-staged.config.js` & `voici-0.4.1/lint-staged.config.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/package.json` & `voici-0.4.1/package.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/tsconfigbase.json` & `voici-0.4.1/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/yarn.lock` & `voici-0.4.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/demo/notebooks/iris.csv` & `voici-0.4.1/demo/notebooks/iris.csv`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/demo/notebooks/voici.ipynb` & `voici-0.4.1/demo/notebooks/voici.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/demo/notebooks/widgets/bqplot.ipynb` & `voici-0.4.1/demo/notebooks/widgets/bqplot.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/demo/notebooks/widgets/ipycanvas.ipynb` & `voici-0.4.1/demo/notebooks/widgets/ipycanvas.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/docs/conf.py` & `voici-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/docs/configuration.md` & `voici-0.4.1/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/docs/deploy.md` & `voici-0.4.1/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/docs/index.md` & `voici-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/docs/install.md` & `voici-0.4.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/docs/voila-logo.svg` & `voici-0.4.1/docs/voila-logo.svg`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/scripts/bump-version.py` & `voici-0.4.1/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/package.json` & `voici-0.4.1/ui-tests/package.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/yarn.lock` & `voici-0.4.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts` & `voici-0.4.1/ui-tests/tests/voici.test.ts`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png` & `voici-0.4.1/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/_version.py` & `voici-0.4.1/voici/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Distributed under the terms of the Modified BSD License.
 
 import re
 
 from collections import namedtuple
 
 # Use "hatch version xx.yy.zz" to handle version changes
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 # PEP440 version parser
 _version_regex = re.compile(
     r"""
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `voici-0.4.0/voici/addon.py` & `voici-0.4.1/voici/addon.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/app.py` & `voici-0.4.1/voici/app.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/exporter.py` & `voici-0.4.1/voici/exporter.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/tree_exporter.py` & `voici-0.4.1/voici/tree_exporter.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1023.js` & `voici-0.4.1/voici/static/build/1023.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1024.js` & `voici-0.4.1/voici/static/build/1024.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/103.js` & `voici-0.4.1/voici/static/build/103.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1053.js` & `voici-0.4.1/voici/static/build/1053.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1058.js` & `voici-0.4.1/voici/static/build/1058.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1100.js` & `voici-0.4.1/voici/static/build/1100.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1105.js` & `voici-0.4.1/voici/static/build/1105.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1432.js` & `voici-0.4.1/voici/static/build/1432.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1553.js` & `voici-0.4.1/voici/static/build/1553.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1581.js` & `voici-0.4.1/voici/static/build/1581.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1667.js` & `voici-0.4.1/voici/static/build/1667.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1672.js` & `voici-0.4.1/voici/static/build/1672.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1770.js` & `voici-0.4.1/voici/static/build/1770.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1890.js` & `voici-0.4.1/voici/static/build/1890.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/1980.js` & `voici-0.4.1/voici/static/build/1980.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2075.js` & `voici-0.4.1/voici/static/build/2075.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2106.js` & `voici-0.4.1/voici/static/build/2106.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2230.js` & `voici-0.4.1/voici/static/build/2230.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2322.js` & `voici-0.4.1/voici/static/build/2322.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2359.js` & `voici-0.4.1/voici/static/build/2359.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2361.js` & `voici-0.4.1/voici/static/build/2361.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2488.js` & `voici-0.4.1/voici/static/build/2488.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2630.js` & `voici-0.4.1/voici/static/build/2630.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2687.js` & `voici-0.4.1/voici/static/build/2687.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/275.js` & `voici-0.4.1/voici/static/build/275.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2784.js` & `voici-0.4.1/voici/static/build/2784.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/286.js` & `voici-0.4.1/voici/static/build/286.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/2950.js` & `voici-0.4.1/voici/static/build/2950.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3008.js` & `voici-0.4.1/voici/static/build/3008.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3086.js` & `voici-0.4.1/voici/static/build/3086.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3251.js` & `voici-0.4.1/voici/static/build/3251.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3256.js` & `voici-0.4.1/voici/static/build/3256.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/330.js` & `voici-0.4.1/voici/static/build/330.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3305.js` & `voici-0.4.1/voici/static/build/3305.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3312.js` & `voici-0.4.1/voici/static/build/3312.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3316.js` & `voici-0.4.1/voici/static/build/3316.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3316.js.LICENSE.txt` & `voici-0.4.1/voici/static/build/3316.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3349.js` & `voici-0.4.1/voici/static/build/3349.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/339.js` & `voici-0.4.1/voici/static/build/339.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -289,15 +289,15 @@
             }(f || (f = {})),
             function(e) {
                 e.onFocus = function(e) {
                     const t = e.target.parentElement;
                     t && ("focus" === e.type ? t.classList.add("jp-mod-focused") : t.classList.remove("jp-mod-focused"))
                 }
             }(_ || (_ = {}));
-            var C = n(28316);
+            var C = n(24627);
             class x extends l.Widget {
                 static create(e) {
                     return new class extends x {
                         render() {
                             return e
                         }
                     }
```

### Comparing `voici-0.4.0/voici/static/build/3504.js` & `voici-0.4.1/voici/static/build/3504.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3655.js` & `voici-0.4.1/voici/static/build/3655.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3693.js` & `voici-0.4.1/voici/static/build/3693.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3811.js` & `voici-0.4.1/voici/static/build/3811.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3851.js` & `voici-0.4.1/voici/static/build/3851.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/3922.js` & `voici-0.4.1/voici/static/build/3922.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4259.js` & `voici-0.4.1/voici/static/build/4259.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4359.js` & `voici-0.4.1/voici/static/build/4359.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4382.js` & `voici-0.4.1/voici/static/build/4382.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/450.js` & `voici-0.4.1/voici/static/build/450.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4530.js` & `voici-0.4.1/voici/static/build/4530.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4875.js` & `voici-0.4.1/voici/static/build/4875.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4896.js` & `voici-0.4.1/voici/static/build/4896.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4939.js` & `voici-0.4.1/voici/static/build/4939.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4963.js` & `voici-0.4.1/voici/static/build/4963.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2776,15 +2776,15 @@
 
             function Fa(e) {
                 return null != e && e instanceof Element && null != e.closest(".".concat(C))
             }
             "undefined" != typeof window && "undefined" != typeof document && n(61722);
             var Ga = n(72779),
                 ja = n.n(Ga),
-                Ka = n(28316),
+                Ka = n(24627),
                 Wa = n(46847);
 
             function Ya() {
                 return Ya = Object.assign ? Object.assign.bind() : function(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var n = arguments[t];
                         for (var c in n) Object.prototype.hasOwnProperty.call(n, c) && (e[c] = n[c])
@@ -13870,146 +13870,147 @@
                 }
             }
             t.default = c.default.createContext || o.default, e.exports = t.default
         },
         74963: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
-                Button: () => O,
-                Checkbox: () => I,
-                Collapse: () => R,
-                CommandPaletteSvg: () => Ht,
-                ContextMenuSvg: () => Nt,
-                DEFAULT_STYLE_CLASS: () => ft,
-                DockPanelSvg: () => bt,
-                FormComponentRegistry: () => Dt,
-                HTMLSelect: () => zt,
-                HTML_SELECT_CLASS: () => Et,
-                IFormComponentRegistry: () => xt,
-                ILabIconManager: () => Pt,
-                IRankedMenu: () => gt,
-                InputGroup: () => H,
-                Intent: () => y.Intent,
-                LabIcon: () => A,
-                MenuSvg: () => It,
-                RankedMenu: () => At,
-                Select: () => N,
-                Switch: () => Tt,
-                TabBarSvg: () => St,
-                TabPanelSvg: () => wt,
-                addAboveIcon: () => V,
-                addBelowIcon: () => S,
-                addIcon: () => b,
-                badIcon: () => M,
-                bellIcon: () => w,
-                blankIcon: () => T,
-                bugDotIcon: () => P,
-                bugIcon: () => D,
-                buildIcon: () => x,
-                caretDownEmptyIcon: () => B,
-                caretDownEmptyThinIcon: () => k,
-                caretDownIcon: () => U,
-                caretLeftIcon: () => F,
-                caretRightIcon: () => G,
-                caretUpEmptyThinIcon: () => j,
-                caretUpIcon: () => K,
-                caseSensitiveIcon: () => W,
-                checkIcon: () => Y,
-                circleEmptyIcon: () => X,
-                circleIcon: () => q,
-                classes: () => z,
-                classesDedupe: () => g,
-                clearIcon: () => Z,
-                closeIcon: () => Q,
-                codeIcon: () => $,
-                consoleIcon: () => J,
-                copyIcon: () => ee,
-                copyrightIcon: () => te,
-                cutIcon: () => ne,
-                deleteIcon: () => ce,
-                downloadIcon: () => oe,
-                duplicateIcon: () => ae,
-                editIcon: () => re,
-                ellipsesIcon: () => se,
-                extensionIcon: () => le,
-                fastForwardIcon: () => ie,
-                fileIcon: () => he,
-                fileUploadIcon: () => pe,
-                filterListIcon: () => ue,
-                folderFavoriteIcon: () => ve,
-                folderIcon: () => de,
-                getReactAttrs: () => _,
-                homeIcon: () => me,
-                html5Icon: () => fe,
-                imageIcon: () => Ee,
-                inspectorIcon: () => ze,
-                jsonIcon: () => ge,
-                juliaIcon: () => _e,
-                jupyterFaviconIcon: () => Le,
-                jupyterIcon: () => Ce,
-                jupyterlabWordmarkIcon: () => Ae,
-                kernelIcon: () => Me,
-                keyboardIcon: () => Te,
-                launchIcon: () => ye,
-                launcherIcon: () => Oe,
-                lineFormIcon: () => He,
-                linkIcon: () => Re,
-                listIcon: () => Ne,
-                listingsInfoIcon: () => Ie,
-                markdownIcon: () => Ve,
-                moveDownIcon: () => Se,
-                moveUpIcon: () => be,
-                newFolderIcon: () => we,
-                notTrustedIcon: () => Pe,
-                notebookIcon: () => De,
-                numberingIcon: () => xe,
-                offlineBoltIcon: () => Be,
-                paletteIcon: () => ke,
-                pasteIcon: () => Ue,
-                pdfIcon: () => Fe,
-                pythonIcon: () => Ge,
-                rKernelIcon: () => je,
-                reactIcon: () => Ke,
-                redoIcon: () => We,
-                refreshIcon: () => Ye,
-                regexIcon: () => Xe,
-                runIcon: () => qe,
-                runningIcon: () => Ze,
-                saveIcon: () => Qe,
-                searchIcon: () => $e,
-                settingsIcon: () => Je,
-                shareIcon: () => et,
-                spreadsheetIcon: () => tt,
-                stopIcon: () => nt,
-                tabIcon: () => ct,
-                tableRowsIcon: () => ot,
-                tagIcon: () => at,
-                terminalIcon: () => rt,
-                textEditorIcon: () => st,
-                tocIcon: () => lt,
-                treeViewIcon: () => it,
-                trustedIcon: () => ht,
-                undoIcon: () => pt,
-                userIcon: () => ut,
-                usersIcon: () => vt,
-                vegaIcon: () => dt,
-                yamlIcon: () => mt
+                Button: () => H,
+                Checkbox: () => V,
+                Collapse: () => N,
+                CommandPaletteSvg: () => Rt,
+                ContextMenuSvg: () => It,
+                DEFAULT_STYLE_CLASS: () => Et,
+                DockPanelSvg: () => wt,
+                FormComponentRegistry: () => xt,
+                HTMLSelect: () => gt,
+                HTML_SELECT_CLASS: () => zt,
+                IFormComponentRegistry: () => Bt,
+                ILabIconManager: () => Dt,
+                IRankedMenu: () => _t,
+                InputGroup: () => R,
+                Intent: () => O.Intent,
+                LabIcon: () => M,
+                MenuSvg: () => Vt,
+                RankedMenu: () => Mt,
+                Select: () => I,
+                Switch: () => yt,
+                TabBarSvg: () => bt,
+                TabPanelSvg: () => Pt,
+                addAboveIcon: () => S,
+                addBelowIcon: () => b,
+                addIcon: () => w,
+                badIcon: () => T,
+                bellIcon: () => P,
+                blankIcon: () => y,
+                bugDotIcon: () => D,
+                bugIcon: () => x,
+                buildIcon: () => B,
+                caretDownEmptyIcon: () => k,
+                caretDownEmptyThinIcon: () => U,
+                caretDownIcon: () => F,
+                caretLeftIcon: () => G,
+                caretRightIcon: () => j,
+                caretUpEmptyThinIcon: () => K,
+                caretUpIcon: () => W,
+                caseSensitiveIcon: () => Y,
+                checkIcon: () => X,
+                circleEmptyIcon: () => q,
+                circleIcon: () => Z,
+                classes: () => g,
+                classesDedupe: () => _,
+                clearIcon: () => Q,
+                closeIcon: () => $,
+                codeIcon: () => J,
+                consoleIcon: () => ee,
+                copyIcon: () => te,
+                copyrightIcon: () => ne,
+                cutIcon: () => ce,
+                deleteIcon: () => oe,
+                downloadIcon: () => ae,
+                duplicateIcon: () => re,
+                editIcon: () => se,
+                ellipsesIcon: () => le,
+                extensionIcon: () => ie,
+                fastForwardIcon: () => he,
+                fileIcon: () => pe,
+                fileUploadIcon: () => ue,
+                filterListIcon: () => ve,
+                folderFavoriteIcon: () => de,
+                folderIcon: () => me,
+                getReactAttrs: () => L,
+                homeIcon: () => fe,
+                html5Icon: () => Ee,
+                imageIcon: () => ze,
+                inspectorIcon: () => ge,
+                jsonIcon: () => _e,
+                juliaIcon: () => Le,
+                jupyterFaviconIcon: () => Ce,
+                jupyterIcon: () => Ae,
+                jupyterlabWordmarkIcon: () => Me,
+                kernelIcon: () => Te,
+                keyboardIcon: () => ye,
+                launchIcon: () => Oe,
+                launcherIcon: () => He,
+                lineFormIcon: () => Re,
+                linkIcon: () => Ne,
+                listIcon: () => Ie,
+                listingsInfoIcon: () => Ve,
+                markdownIcon: () => Se,
+                moveDownIcon: () => be,
+                moveUpIcon: () => we,
+                newFolderIcon: () => Pe,
+                notTrustedIcon: () => De,
+                notebookIcon: () => xe,
+                numberingIcon: () => Be,
+                offlineBoltIcon: () => ke,
+                paletteIcon: () => Ue,
+                pasteIcon: () => Fe,
+                pdfIcon: () => Ge,
+                pythonIcon: () => je,
+                rKernelIcon: () => Ke,
+                reactIcon: () => We,
+                redoIcon: () => Ye,
+                refreshIcon: () => Xe,
+                regexIcon: () => qe,
+                runIcon: () => Ze,
+                runningIcon: () => Qe,
+                saveIcon: () => $e,
+                searchIcon: () => Je,
+                settingsIcon: () => et,
+                shareIcon: () => tt,
+                spreadsheetIcon: () => nt,
+                stopIcon: () => ct,
+                tabIcon: () => ot,
+                tableRowsIcon: () => at,
+                tagIcon: () => rt,
+                terminalIcon: () => st,
+                textEditorIcon: () => lt,
+                tocIcon: () => it,
+                treeViewIcon: () => ht,
+                trustedIcon: () => pt,
+                undoIcon: () => ut,
+                userIcon: () => vt,
+                usersIcon: () => dt,
+                vegaIcon: () => mt,
+                yamlIcon: () => ft
             });
             var c = n(93920),
                 o = n(74410),
                 a = n(76669),
                 r = n(58539),
                 s = n(9297),
                 l = n(97505),
                 i = n.n(l),
                 h = n(92233),
                 p = n(4947),
-                u = n(28316);
-            const v = '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 18 18">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M9 13.5c-2.49 0-4.5-2.01-4.5-4.5S6.51 4.5 9 4.5c1.24 0 2.36.52 3.17 1.33L10 8h5V3l-1.76 1.76C12.15 3.68 10.66 3 9 3 5.69 3 3.01 5.69 3.01 9S5.69 15 9 15c2.97 0 5.43-2.16 5.9-5h-1.52c-.46 2-2.24 3.5-4.38 3.5z"/>\n    </g>\n</svg>\n';
-            var d, m = n(66770);
+                u = n(24627),
+                v = n.n(u);
+            const d = '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 18 18">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M9 13.5c-2.49 0-4.5-2.01-4.5-4.5S6.51 4.5 9 4.5c1.24 0 2.36.52 3.17 1.33L10 8h5V3l-1.76 1.76C12.15 3.68 10.66 3 9 3 5.69 3 3.01 5.69 3.01 9S5.69 15 9 15c2.97 0 5.43-2.16 5.9-5h-1.52c-.46 2-2.24 3.5-4.38 3.5z"/>\n    </g>\n</svg>\n';
+            var m, f = n(66770);
             ! function(e) {
                 const t = {
                     breadCrumb: {
                         container: {
                             $nest: {
                                 "&:first-child svg": {
                                     bottom: "1px",
@@ -14343,133 +14344,133 @@
                     const d = function(e) {
                         return e ? (Array.isArray(e) || (e = [e]), e.map((e => "string" == typeof e ? t[e] : e))) : []
                     }(s);
                     d.push({
                         element: h,
                         options: p
                     });
-                    const f = function(e) {
+                    const m = function(e) {
                         var t;
-                        return (0, m.oB)(Object.assign(Object.assign({}, e.container), {
+                        return (0, f.oB)(Object.assign(Object.assign({}, e.container), {
                             $nest: Object.assign(Object.assign({}, null === (t = e.container) || void 0 === t ? void 0 : t.$nest), {
                                 svg: e.element
                             })
                         }))
                     }(function(e) {
                         const t = Object.assign({}, ...e.map((e => e.options)));
                         return t.elementPosition && e.unshift(c[t.elementPosition]), t.elementSize && e.unshift(a[t.elementSize]),
                             function(e) {
                                 return {
                                     container: Object.assign({}, ...e.map((e => e.container))),
                                     element: Object.assign({}, ...e.map((e => e.element)))
                                 }
                             }(e)
                     }(d));
-                    return u && r.set(v, f), f
+                    return u && r.set(v, m), m
                 }
-            }(d || (d = {}));
-            var f = n(59110);
+            }(m || (m = {}));
+            var E = n(59110);
 
-            function E(e) {
+            function z(e) {
                 return e.map((e => e && "object" == typeof e ? Object.keys(e).map((t => !!e[t] && t)) : "string" == typeof e ? e.split(/\s+/) : [])).reduce(((e, t) => e.concat(t)), []).filter((e => !!e))
             }
 
-            function z(...e) {
-                return E(e).join(" ")
+            function g(...e) {
+                return z(e).join(" ")
             }
 
-            function g(...e) {
-                return [...new Set(E(e))].join(" ")
+            function _(...e) {
+                return [...new Set(z(e))].join(" ")
             }
 
-            function _(e, {
+            function L(e, {
                 ignore: t = []
             } = {}) {
-                return e.getAttributeNames().reduce(((n, c) => ("style" === c || t.includes(c) || (c.startsWith("data") ? n[c] = e.getAttribute(c) : n[f.Text.camelCase(c)] = e.getAttribute(c)), n)), {})
+                return e.getAttributeNames().reduce(((n, c) => ("style" === c || t.includes(c) || (c.startsWith("data") ? n[c] = e.getAttribute(c) : n[E.Text.camelCase(c)] = e.getAttribute(c)), n)), {})
             }
-            var L, C = function(e, t) {
+            var C, A = function(e, t) {
                 var n = {};
                 for (var c in e) Object.prototype.hasOwnProperty.call(e, c) && t.indexOf(c) < 0 && (n[c] = e[c]);
                 if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                     var o = 0;
                     for (c = Object.getOwnPropertySymbols(e); o < c.length; o++) t.indexOf(c[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, c[o]) && (n[c[o]] = e[c[o]])
                 }
                 return n
             };
-            class A {
+            class M {
                 constructor({
                     name: e,
                     svgstr: t,
                     render: n,
                     unrender: c,
                     _loading: o = !1
                 }) {
-                    if (this._props = {}, this._svgReplaced = new p.Signal(this), this._svgElement = void 0, this._svgInnerHTML = void 0, this._svgReactAttrs = void 0, !e || !t) return console.error(`When defining a new LabIcon, name and svgstr must both be non-empty strings. name: ${e}, svgstr: ${t}`), M;
-                    if (this._loading = o, A._instances.has(e)) {
-                        const n = A._instances.get(e);
-                        return this._loading ? (n.svgstr = t, this._loading = !1, n) : (A._debug && console.warn(`Redefining previously loaded icon svgstr. name: ${e}, svgstrOld: ${n.svgstr}, svgstr: ${t}`), n.svgstr = t, n)
+                    if (this._props = {}, this._svgReplaced = new p.Signal(this), this._svgElement = void 0, this._svgInnerHTML = void 0, this._svgReactAttrs = void 0, !e || !t) return console.error(`When defining a new LabIcon, name and svgstr must both be non-empty strings. name: ${e}, svgstr: ${t}`), T;
+                    if (this._loading = o, M._instances.has(e)) {
+                        const n = M._instances.get(e);
+                        return this._loading ? (n.svgstr = t, this._loading = !1, n) : (M._debug && console.warn(`Redefining previously loaded icon svgstr. name: ${e}, svgstrOld: ${n.svgstr}, svgstr: ${t}`), n.svgstr = t, n)
                     }
                     this.name = e, this.react = this._initReact(e), this.svgstr = t, this._initRender({
                         render: n,
                         unrender: c
-                    }), A._instances.set(this.name, this)
+                    }), M._instances.set(this.name, this)
                 }
                 static remove(e) {
                     for (; e.firstChild;) e.firstChild.remove();
                     return e.className = "", e
                 }
                 static resolve({
                     icon: e
                 }) {
-                    if (e instanceof A) return e;
+                    if (e instanceof M) return e;
                     if ("string" == typeof e) {
-                        return A._instances.get(e) || (A._debug && console.warn(`Lookup failed for icon, creating loading icon. icon: ${e}`), new A({
+                        return M._instances.get(e) || (M._debug && console.warn(`Lookup failed for icon, creating loading icon. icon: ${e}`), new M({
                             name: e,
-                            svgstr: v,
+                            svgstr: d,
                             _loading: !0
                         }))
                     }
-                    return new A(e)
+                    return new M(e)
                 }
                 static resolveElement(e) {
                     var {
                         icon: t,
                         iconClass: n,
                         fallback: c
-                    } = e, o = C(e, ["icon", "iconClass", "fallback"]);
-                    return L.isResolvable(t) ? A.resolve({
+                    } = e, o = A(e, ["icon", "iconClass", "fallback"]);
+                    return C.isResolvable(t) ? M.resolve({
                         icon: t
-                    }).element(o) : !n && c ? c.element(o) : (o.className = z(n, o.className), L.blankElement(o))
+                    }).element(o) : !n && c ? c.element(o) : (o.className = g(n, o.className), C.blankElement(o))
                 }
                 static resolveReact(e) {
                     var {
                         icon: t,
                         iconClass: n,
                         fallback: c
-                    } = e, o = C(e, ["icon", "iconClass", "fallback"]);
-                    if (!L.isResolvable(t)) return !n && c ? i().createElement(c.react, Object.assign({}, o)) : (o.className = z(n, o.className), i().createElement(L.blankReact, Object.assign({}, o)));
-                    const a = A.resolve({
+                    } = e, o = A(e, ["icon", "iconClass", "fallback"]);
+                    if (!C.isResolvable(t)) return !n && c ? i().createElement(c.react, Object.assign({}, o)) : (o.className = g(n, o.className), i().createElement(C.blankReact, Object.assign({}, o)));
+                    const a = M.resolve({
                         icon: t
                     });
                     return i().createElement(a.react, Object.assign({}, o))
                 }
                 static resolveSvg({
                     name: e,
                     svgstr: t
                 }) {
-                    const n = (new DOMParser).parseFromString(L.svgstrShim(t), "image/svg+xml"),
+                    const n = (new DOMParser).parseFromString(C.svgstrShim(t), "image/svg+xml"),
                         c = n.querySelector("parsererror");
                     if (c) {
                         const n = `SVG HTML was malformed for LabIcon instance.\nname: ${e}, svgstr: ${t}`;
-                        return A._debug ? (console.error(n), c) : (console.warn(n), null)
+                        return M._debug ? (console.error(n), c) : (console.warn(n), null)
                     }
                     return n.documentElement
                 }
                 static toggleDebug(e) {
-                    A._debug = null != e ? e : !A._debug
+                    M._debug = null != e ? e : !M._debug
                 }
                 bindprops(e) {
                     const t = Object.create(this);
                     return t._props = e, t.react = t._initReact(t.name + "_bind"), t
                 }
                 element(e = {}) {
                     var t;
@@ -14477,23 +14478,23 @@
                         {
                             className: c,
                             container: o,
                             label: a,
                             title: r,
                             tag: s = "div"
                         } = n,
-                        l = C(n, ["className", "container", "label", "title", "tag"]);
+                        l = A(n, ["className", "container", "label", "title", "tag"]);
                     const i = null == o ? void 0 : o.firstChild;
                     if ((null === (t = null == i ? void 0 : i.dataset) || void 0 === t ? void 0 : t.iconId) === this._uuid) return i;
                     if (!this.svgElement) return document.createElement("div");
                     let h = !0;
                     if (o)
                         for (; o.firstChild;) o.firstChild.remove();
                     else o = document.createElement(s), h = !1;
-                    null != a && (o.textContent = a), L.initContainer({
+                    null != a && (o.textContent = a), C.initContainer({
                         container: o,
                         className: c,
                         styleProps: l,
                         title: r
                     });
                     const p = this.svgElement.cloneNode(!0);
                     return o.appendChild(p), h ? p : o
@@ -14511,15 +14512,15 @@
                         uuid: this._uuid
                     })), this._svgElement
                 }
                 get svgInnerHTML() {
                     return void 0 === this._svgInnerHTML && (null === this.svgElement ? this._svgInnerHTML = null : this._svgInnerHTML = this.svgElement.innerHTML), this._svgInnerHTML
                 }
                 get svgReactAttrs() {
-                    return void 0 === this._svgReactAttrs && (null === this.svgElement ? this._svgReactAttrs = null : this._svgReactAttrs = _(this.svgElement, {
+                    return void 0 === this._svgReactAttrs && (null === this.svgElement ? this._svgReactAttrs = null : this._svgReactAttrs = L(this.svgElement, {
                         ignore: ["data-icon-id"]
                     })), this._svgReactAttrs
                 }
                 get svgstr() {
                     return this._svgstr
                 }
                 set svgstr(e) {
@@ -14536,15 +14537,15 @@
                             {
                                 className: c,
                                 container: o,
                                 label: a,
                                 title: r,
                                 tag: s = "div"
                             } = n,
-                            l = C(n, ["className", "container", "label", "title", "tag"]),
+                            l = A(n, ["className", "container", "label", "title", "tag"]),
                             [, h] = i().useState(this._uuid);
                         i().useEffect((() => {
                             const e = () => {
                                 h(this._uuid)
                             };
                             return this._svgReplaced.connect(e), () => {
                                 this._svgReplaced.disconnect(e)
@@ -14554,63 +14555,63 @@
                         if (!this.svgInnerHTML || !this.svgReactAttrs) return i().createElement(i().Fragment, null);
                         const u = i().createElement("svg", Object.assign({}, this.svgReactAttrs, {
                             dangerouslySetInnerHTML: {
                                 __html: this.svgInnerHTML
                             },
                             ref: t
                         }));
-                        return o ? (L.initContainer({
+                        return o ? (C.initContainer({
                             container: o,
                             className: c,
                             styleProps: l,
                             title: r
                         }), i().createElement(i().Fragment, null, u, a)) : i().createElement(p, {
-                            className: z(c, d.styleClass(l))
+                            className: g(c, m.styleClass(l))
                         }, u, a)
                     }));
                     return t.displayName = `LabIcon_${e}`, t
                 }
                 _initRender({
                     render: e,
                     unrender: t
                 }) {
                     e ? (this.render = e, t && (this.unrender = t)) : t && console.warn("In _initRender, ignoring unrender arg since render is undefined")
                 }
                 _initSvg({
                     title: e,
                     uuid: t
                 } = {}) {
-                    const n = A.resolveSvg(this);
-                    return n ? ("parsererror" !== n.tagName && (n.dataset.icon = this.name, t && (n.dataset.iconId = t), e && L.setTitleSvg(n, e)), n) : n
+                    const n = M.resolveSvg(this);
+                    return n ? ("parsererror" !== n.tagName && (n.dataset.icon = this.name, t && (n.dataset.iconId = t), e && C.setTitleSvg(n, e)), n) : n
                 }
             }
-            A._debug = !1, A._instances = new Map,
+            M._debug = !1, M._instances = new Map,
                 function(e) {
                     function t({
                         container: e,
                         className: t,
                         styleProps: n,
                         title: c
                     }) {
                         null != c && (e.title = c);
-                        const o = d.styleClass(n);
+                        const o = m.styleClass(n);
                         if (null != t) {
-                            const n = z(t, o);
+                            const n = g(t, o);
                             return e.className = n, n
                         }
                         return o ? (e.classList.add(o), o) : ""
                     }
                     e.blankElement = function(t) {
                         var {
                             className: n = "",
                             container: c,
                             label: o,
                             title: a,
                             tag: r = "div"
-                        } = t, s = C(t, ["className", "container", "label", "title", "tag"]);
+                        } = t, s = A(t, ["className", "container", "label", "title", "tag"]);
                         if ((null == c ? void 0 : c.className) === n) return c;
                         if (c)
                             for (; c.firstChild;) c.firstChild.remove();
                         else c = document.createElement(r);
                         return null != o && (c.textContent = o), e.initContainer({
                             container: c,
                             className: n,
@@ -14620,24 +14621,24 @@
                     }, e.blankReact = i().forwardRef(((e, n) => {
                         var {
                             className: c = "",
                             container: o,
                             label: a,
                             title: r,
                             tag: s = "div"
-                        } = e, l = C(e, ["className", "container", "label", "title", "tag"]);
+                        } = e, l = A(e, ["className", "container", "label", "title", "tag"]);
                         const h = s;
                         return o ? (t({
                             container: o,
                             className: c,
                             styleProps: l,
                             title: r
                         }), i().createElement(i().Fragment, null)) : i().createElement(h, {
-                            className: z(c, d.styleClass(l))
-                        }, n && T.react({
+                            className: g(c, m.styleClass(l))
+                        }, n && y.react({
                             ref: n
                         }), a)
                     })), e.blankReact.displayName = "BlankReact", e.initContainer = t, e.isResolvable = function(e) {
                         return !(!e || !("string" == typeof e || e.name && e.svgstr))
                     }, e.setTitleSvg = function(e, t) {
                         const n = e.getElementsByTagName("title");
                         if (n.length) n[0].textContent = t;
@@ -14664,446 +14665,446 @@
                                 label: o
                             }, null === (c = this._rendererOptions) || void 0 === c ? void 0 : c.props), null == t ? void 0 : t.props))
                         }
                     }, e.ReactRenderer = class extends n {
                         render(e, t) {
                             var n, c;
                             let o = null === (n = null == t ? void 0 : t.children) || void 0 === n ? void 0 : n[0];
-                            "string" != typeof o && (o = void 0), u.render(i().createElement(this._icon.react, Object.assign({
+                            "string" != typeof o && (o = void 0), v().render(i().createElement(this._icon.react, Object.assign({
                                 container: e,
                                 label: o
                             }, Object.assign(Object.assign({}, null === (c = this._rendererOptions) || void 0 === c ? void 0 : c.props), null == t ? void 0 : t.props))), e)
                         }
                         unrender(e) {
-                            u.unmountComponentAtNode(e)
+                            v().unmountComponentAtNode(e)
                         }
                     }
-                }(L || (L = {}));
-            const M = new A({
+                }(C || (C = {}));
+            const T = new M({
                     name: "ui-components:bad",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">\n    <path\n        class="jp-icon0"\n        fill="#000"\n        d="M24 20.188l-8.315-8.209 8.2-8.282-3.697-3.697-8.212 8.318-8.31-8.203-3.666 3.666 8.321 8.24-8.206 8.313 3.666 3.666 8.237-8.318 8.285 8.203z"\n    />\n</svg>\n'
                 }),
-                T = new A({
+                y = new M({
                     name: "ui-components:blank",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">\n    <path\n        fill="#000"\n        fill-opacity="0.0"\n        d="M24 20.188l-8.315-8.209 8.2-8.282-3.697-3.697-8.212 8.318-8.31-8.203-3.666 3.666 8.321 8.24-8.206 8.313 3.666 3.666 8.237-8.318 8.285 8.203z"\n    />\n</svg>\n'
                 });
-            var y = n(9382);
-            const O = e => l.createElement(c.zx, Object.assign({}, e, {
-                    className: z(e.className, e.minimal ? "minimal" : "", "jp-Button")
+            var O = n(9382);
+            const H = e => l.createElement(c.zx, Object.assign({}, e, {
+                    className: g(e.className, e.minimal ? "minimal" : "", "jp-Button")
                 })),
-                H = e => e.rightIcon ? l.createElement(r.B, Object.assign({}, e, {
-                    className: z(e.className, "jp-InputGroup"),
+                R = e => e.rightIcon ? l.createElement(r.B, Object.assign({}, e, {
+                    className: g(e.className, "jp-InputGroup"),
                     rightElement: l.createElement("div", {
                         className: "jp-InputGroupAction"
-                    }, l.createElement(A.resolveReact, {
+                    }, l.createElement(M.resolveReact, {
                         icon: e.rightIcon
                     }))
                 })) : l.createElement(r.B, Object.assign({}, e, {
-                    className: z(e.className, "jp-InputGroup")
+                    className: g(e.className, "jp-InputGroup")
                 })),
-                R = e => l.createElement(o.UO, Object.assign({}, e)),
-                N = e => l.createElement(s.P, Object.assign({}, e, {
-                    className: z(e.className, "jp-Select")
+                N = e => l.createElement(o.UO, Object.assign({}, e)),
+                I = e => l.createElement(s.P, Object.assign({}, e, {
+                    className: g(e.className, "jp-Select")
                 })),
-                I = e => l.createElement(a.XZ, Object.assign({}, e, {
-                    className: z(e.className, "jp-Checkbox")
+                V = e => l.createElement(a.XZ, Object.assign({}, e, {
+                    className: g(e.className, "jp-Checkbox")
                 })),
-                V = new A({
+                S = new M({
                     name: "ui-components:add-above",
                     svgstr: '<svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">\n<g clip-path="url(#clip0_137_19492)">\n<path class="jp-icon3" d="M4.75 4.93066H6.625V6.80566C6.625 7.01191 6.79375 7.18066 7 7.18066C7.20625 7.18066 7.375 7.01191 7.375 6.80566V4.93066H9.25C9.45625 4.93066 9.625 4.76191 9.625 4.55566C9.625 4.34941 9.45625 4.18066 9.25 4.18066H7.375V2.30566C7.375 2.09941 7.20625 1.93066 7 1.93066C6.79375 1.93066 6.625 2.09941 6.625 2.30566V4.18066H4.75C4.54375 4.18066 4.375 4.34941 4.375 4.55566C4.375 4.76191 4.54375 4.93066 4.75 4.93066Z" fill="#616161" stroke="#616161" stroke-width="0.7"/>\n</g>\n<path class="jp-icon3" fill-rule="evenodd" clip-rule="evenodd" d="M11.5 9.5V11.5L2.5 11.5V9.5L11.5 9.5ZM12 8C12.5523 8 13 8.44772 13 9V12C13 12.5523 12.5523 13 12 13L2 13C1.44772 13 1 12.5523 1 12V9C1 8.44772 1.44771 8 2 8L12 8Z" fill="#616161"/>\n<defs>\n<clipPath id="clip0_137_19492">\n<rect class="jp-icon3" width="6" height="6" fill="white" transform="matrix(-1 0 0 1 10 1.55566)"/>\n</clipPath>\n</defs>\n</svg>\n'
                 }),
-                S = new A({
+                b = new M({
                     name: "ui-components:add-below",
                     svgstr: '<svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">\n<g clip-path="url(#clip0_137_19498)">\n<path class="jp-icon3" d="M9.25 10.0693L7.375 10.0693L7.375 8.19434C7.375 7.98809 7.20625 7.81934 7 7.81934C6.79375 7.81934 6.625 7.98809 6.625 8.19434L6.625 10.0693L4.75 10.0693C4.54375 10.0693 4.375 10.2381 4.375 10.4443C4.375 10.6506 4.54375 10.8193 4.75 10.8193L6.625 10.8193L6.625 12.6943C6.625 12.9006 6.79375 13.0693 7 13.0693C7.20625 13.0693 7.375 12.9006 7.375 12.6943L7.375 10.8193L9.25 10.8193C9.45625 10.8193 9.625 10.6506 9.625 10.4443C9.625 10.2381 9.45625 10.0693 9.25 10.0693Z" fill="#616161" stroke="#616161" stroke-width="0.7"/>\n</g>\n<path class="jp-icon3" fill-rule="evenodd" clip-rule="evenodd" d="M2.5 5.5L2.5 3.5L11.5 3.5L11.5 5.5L2.5 5.5ZM2 7C1.44772 7 1 6.55228 1 6L1 3C1 2.44772 1.44772 2 2 2L12 2C12.5523 2 13 2.44772 13 3L13 6C13 6.55229 12.5523 7 12 7L2 7Z" fill="#616161"/>\n<defs>\n<clipPath id="clip0_137_19498">\n<rect class="jp-icon3" width="6" height="6" fill="white" transform="matrix(1 1.74846e-07 1.74846e-07 -1 4 13.4443)"/>\n</clipPath>\n</defs>\n</svg>\n'
                 }),
-                b = new A({
+                w = new M({
                     name: "ui-components:add",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/>\n  </g>\n</svg>\n'
                 }),
-                w = new A({
+                P = new M({
                     name: "ui-components:bell",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 16 16" version="1.1">\n   <path class="jp-icon2 jp-icon-selectable" fill="#333333"\n      d="m8 0.29c-1.4 0-2.7 0.73-3.6 1.8-1.2 1.5-1.4 3.4-1.5 5.2-0.18 2.2-0.44 4-2.3 5.3l0.28 1.3h5c0.026 0.66 0.32 1.1 0.71 1.5 0.84 0.61 2 0.61 2.8 0 0.52-0.4 0.6-1 0.71-1.5h5l0.28-1.3c-1.9-0.97-2.2-3.3-2.3-5.3-0.13-1.8-0.26-3.7-1.5-5.2-0.85-1-2.2-1.8-3.6-1.8zm0 1.4c0.88 0 1.9 0.55 2.5 1.3 0.88 1.1 1.1 2.7 1.2 4.4 0.13 1.7 0.23 3.6 1.3 5.2h-10c1.1-1.6 1.2-3.4 1.3-5.2 0.13-1.7 0.3-3.3 1.2-4.4 0.59-0.72 1.6-1.3 2.5-1.3zm-0.74 12h1.5c-0.0015 0.28 0.015 0.79-0.74 0.79-0.73 0.0016-0.72-0.53-0.74-0.79z" />\n</svg>\n'
                 }),
-                P = new A({
+                D = new M({
                     name: "ui-components:bug-dot",
                     svgstr: '<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">\n    <g class="jp-icon3 jp-icon-selectable" fill="#616161">\n        <path fill-rule="evenodd" clip-rule="evenodd" d="M17.19 8H20V10H17.91C17.96 10.33 18 10.66 18 11V12H20V14H18.5H18V14.0275C15.75 14.2762 14 16.1837 14 18.5C14 19.208 14.1635 19.8779 14.4549 20.4739C13.7063 20.8117 12.8757 21 12 21C9.78 21 7.85 19.79 6.81 18H4V16H6.09C6.04 15.67 6 15.34 6 15V14H4V12H6V11C6 10.66 6.04 10.33 6.09 10H4V8H6.81C7.26 7.22 7.88 6.55 8.62 6.04L7 4.41L8.41 3L10.59 5.17C11.04 5.06 11.51 5 12 5C12.49 5 12.96 5.06 13.42 5.17L15.59 3L17 4.41L15.37 6.04C16.12 6.55 16.74 7.22 17.19 8ZM10 16H14V14H10V16ZM10 12H14V10H10V12Z" fill="#616161"/>\n        <path d="M22 18.5C22 20.433 20.433 22 18.5 22C16.567 22 15 20.433 15 18.5C15 16.567 16.567 15 18.5 15C20.433 15 22 16.567 22 18.5Z" fill="#616161"/>\n    </g>\n</svg>\n'
                 }),
-                D = new A({
+                x = new M({
                     name: "ui-components:bug",
                     svgstr: '<svg viewBox="0 0 24 24" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3 jp-icon-selectable" fill="#616161">\n    <path d="M20 8h-2.81c-.45-.78-1.07-1.45-1.82-1.96L17 4.41 15.59 3l-2.17 2.17C12.96 5.06 12.49 5 12 5c-.49 0-.96.06-1.41.17L8.41 3 7 4.41l1.62 1.63C7.88 6.55 7.26 7.22 6.81 8H4v2h2.09c-.05.33-.09.66-.09 1v1H4v2h2v1c0 .34.04.67.09 1H4v2h2.81c1.04 1.79 2.97 3 5.19 3s4.15-1.21 5.19-3H20v-2h-2.09c.05-.33.09-.66.09-1v-1h2v-2h-2v-1c0-.34-.04-.67-.09-1H20V8zm-6 8h-4v-2h4v2zm0-4h-4v-2h4v2z"/>\n  </g>\n</svg>\n'
                 }),
-                x = new A({
+                B = new M({
                     name: "ui-components:build",
                     svgstr: '<svg width="16" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M14.9 17.45C16.25 17.45 17.35 16.35 17.35 15C17.35 13.65 16.25 12.55 14.9 12.55C13.54 12.55 12.45 13.65 12.45 15C12.45 16.35 13.54 17.45 14.9 17.45ZM20.1 15.68L21.58 16.84C21.71 16.95 21.75 17.13 21.66 17.29L20.26 19.71C20.17 19.86 20 19.92 19.83 19.86L18.09 19.16C17.73 19.44 17.33 19.67 16.91 19.85L16.64 21.7C16.62 21.87 16.47 22 16.3 22H13.5C13.32 22 13.18 21.87 13.15 21.7L12.89 19.85C12.46 19.67 12.07 19.44 11.71 19.16L9.96002 19.86C9.81002 19.92 9.62002 19.86 9.54002 19.71L8.14002 17.29C8.05002 17.13 8.09002 16.95 8.22002 16.84L9.70002 15.68L9.65001 15L9.70002 14.31L8.22002 13.16C8.09002 13.05 8.05002 12.86 8.14002 12.71L9.54002 10.29C9.62002 10.13 9.81002 10.07 9.96002 10.13L11.71 10.84C12.07 10.56 12.46 10.32 12.89 10.15L13.15 8.28998C13.18 8.12998 13.32 7.99998 13.5 7.99998H16.3C16.47 7.99998 16.62 8.12998 16.64 8.28998L16.91 10.15C17.33 10.32 17.73 10.56 18.09 10.84L19.83 10.13C20 10.07 20.17 10.13 20.26 10.29L21.66 12.71C21.75 12.86 21.71 13.05 21.58 13.16L20.1 14.31L20.15 15L20.1 15.68Z"/>\n    <path d="M7.32966 7.44454C8.0831 7.00954 8.33932 6.05332 7.90432 5.29988C7.46932 4.54643 6.5081 4.28156 5.75466 4.71656C5.39176 4.92608 5.12695 5.27118 5.01849 5.67594C4.91004 6.08071 4.96682 6.51198 5.17634 6.87488C5.61134 7.62832 6.57622 7.87954 7.32966 7.44454ZM9.65718 4.79593L10.8672 4.95179C10.9628 4.97741 11.0402 5.07133 11.0382 5.18793L11.0388 6.98893C11.0455 7.10054 10.9616 7.19518 10.855 7.21054L9.66001 7.38083L9.23915 8.13188L9.66961 9.25745C9.70729 9.36271 9.66934 9.47699 9.57408 9.53199L8.01523 10.432C7.91131 10.492 7.79337 10.4677 7.72105 10.3824L6.98748 9.43188L6.10931 9.43083L5.34704 10.3905C5.28909 10.4702 5.17383 10.4905 5.07187 10.4339L3.51245 9.53293C3.41049 9.47633 3.37647 9.35741 3.41075 9.25679L3.86347 8.14093L3.61749 7.77488L3.42347 7.37883L2.23075 7.21297C2.12647 7.19235 2.04049 7.10342 2.04245 6.98682L2.04187 5.18582C2.04383 5.06922 2.11909 4.97958 2.21704 4.96922L3.42065 4.79393L3.86749 4.02788L3.41105 2.91731C3.37337 2.81204 3.41131 2.69776 3.51523 2.63776L5.07408 1.73776C5.16934 1.68276 5.28729 1.70704 5.35961 1.79231L6.11915 2.72788L6.98001 2.73893L7.72496 1.78922C7.79156 1.70458 7.91548 1.67922 8.00879 1.74082L9.56821 2.64182C9.67017 2.69842 9.71285 2.81234 9.68723 2.90797L9.21718 4.03383L9.46316 4.39988L9.65718 4.79593Z"/>\n  </g>\n</svg>\n'
                 }),
-                B = new A({
+                k = new M({
                     name: "ui-components:caret-down-empty",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 18 18">\n  <g class="jp-icon3" fill="#616161" shape-rendering="geometricPrecision">\n    <path d="M5.2,5.9L9,9.7l3.8-3.8l1.2,1.2l-4.9,5l-4.9-5L5.2,5.9z"/>\n  </g>\n</svg>\n'
                 }),
-                k = new A({
+                U = new M({
                     name: "ui-components:caret-down-empty-thin",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 20 20">\n\t<g class="jp-icon3" fill="#616161" shape-rendering="geometricPrecision">\n\t\t<polygon class="st1" points="9.9,13.6 3.6,7.4 4.4,6.6 9.9,12.2 15.4,6.7 16.1,7.4 "/>\n\t</g>\n</svg>\n'
                 }),
-                U = new A({
+                F = new M({
                     name: "ui-components:caret-down",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 18 18">\n  <g class="jp-icon3" fill="#616161" shape-rendering="geometricPrecision">\n    <path d="M5.2,7.5L9,11.2l3.8-3.8H5.2z"/>\n  </g>\n</svg>\n'
                 }),
-                F = new A({
+                G = new M({
                     name: "ui-components:caret-left",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 18 18">\n\t<g class="jp-icon3" fill="#616161" shape-rendering="geometricPrecision">\n\t\t<path d="M10.8,12.8L7.1,9l3.8-3.8l0,7.6H10.8z"/>\n  </g>\n</svg>\n'
                 }),
-                G = new A({
+                j = new M({
                     name: "ui-components:caret-right",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 18 18">\n  <g class="jp-icon3" fill="#616161" shape-rendering="geometricPrecision">\n    <path d="M7.2,5.2L10.9,9l-3.8,3.8V5.2H7.2z"/>\n  </g>\n</svg>\n'
                 }),
-                j = new A({
+                K = new M({
                     name: "ui-components:caret-up-empty-thin",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 20 20">\n\t<g class="jp-icon3" fill="#616161" shape-rendering="geometricPrecision">\n\t\t<polygon class="st1" points="15.4,13.3 9.9,7.7 4.4,13.2 3.6,12.5 9.9,6.3 16.1,12.6 "/>\n\t</g>\n</svg>\n'
                 }),
-                K = new A({
+                W = new M({
                     name: "ui-components:caret-up",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 18 18">\n\t<g class="jp-icon3" fill="#616161" shape-rendering="geometricPrecision">\n\t\t<path d="M5.2,10.5L9,6.8l3.8,3.8H5.2z"/>\n  </g>\n</svg>\n'
                 }),
-                W = new A({
+                Y = new M({
                     name: "ui-components:case-sensitive",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 20 20">\n  <g class="jp-icon2" fill="#414141">\n    <rect x="2" y="2" width="16" height="16"/>\n  </g>\n  <g class="jp-icon-accent2" fill="#FFF">\n    <path d="M7.6,8h0.9l3.5,8h-1.1L10,14H6l-0.9,2H4L7.6,8z M8,9.1L6.4,13h3.2L8,9.1z"/>\n    <path d="M16.6,9.8c-0.2,0.1-0.4,0.1-0.7,0.1c-0.2,0-0.4-0.1-0.6-0.2c-0.1-0.1-0.2-0.4-0.2-0.7 c-0.3,0.3-0.6,0.5-0.9,0.7c-0.3,0.1-0.7,0.2-1.1,0.2c-0.3,0-0.5,0-0.7-0.1c-0.2-0.1-0.4-0.2-0.6-0.3c-0.2-0.1-0.3-0.3-0.4-0.5 c-0.1-0.2-0.1-0.4-0.1-0.7c0-0.3,0.1-0.6,0.2-0.8c0.1-0.2,0.3-0.4,0.4-0.5C12,7,12.2,6.9,12.5,6.8c0.2-0.1,0.5-0.1,0.7-0.2 c0.3-0.1,0.5-0.1,0.7-0.1c0.2,0,0.4-0.1,0.6-0.1c0.2,0,0.3-0.1,0.4-0.2c0.1-0.1,0.2-0.2,0.2-0.4c0-1-1.1-1-1.3-1 c-0.4,0-1.4,0-1.4,1.2h-0.9c0-0.4,0.1-0.7,0.2-1c0.1-0.2,0.3-0.4,0.5-0.6c0.2-0.2,0.5-0.3,0.8-0.3C13.3,4,13.6,4,13.9,4 c0.3,0,0.5,0,0.8,0.1c0.3,0,0.5,0.1,0.7,0.2c0.2,0.1,0.4,0.3,0.5,0.5C16,5,16,5.2,16,5.6v2.9c0,0.2,0,0.4,0,0.5 c0,0.1,0.1,0.2,0.3,0.2c0.1,0,0.2,0,0.3,0V9.8z M15.2,6.9c-1.2,0.6-3.1,0.2-3.1,1.4c0,1.4,3.1,1,3.1-0.5V6.9z"/>\n  </g>\n</svg>\n'
                 }),
-                Y = new A({
+                X = new M({
                     name: "ui-components:check",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3 jp-icon-selectable" fill="#616161">\n    <path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z"/>\n  </g>\n</svg>\n'
                 }),
-                X = new A({
+                q = new M({
                     name: "ui-components:circle-empty",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M12 2C6.47 2 2 6.47 2 12s4.47 10 10 10 10-4.47 10-10S17.53 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8z"/>\n  </g>\n</svg>\n'
                 }),
-                q = new A({
+                Z = new M({
                     name: "ui-components:circle",
                     svgstr: '<svg viewBox="0 0 18 18" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <circle cx="9" cy="9" r="8"/>\n  </g>\n</svg>\n'
                 }),
-                Z = new A({
+                Q = new M({
                     name: "ui-components:clear",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <mask id="donutHole">\n    <rect width="24" height="24" fill="white" />\n    <circle cx="12" cy="12" r="8" fill="black"/>\n  </mask>\n\n  <g class="jp-icon3" fill="#616161">\n    <rect height="18" width="2" x="11" y="3" transform="rotate(315, 12, 12)"/>\n    <circle cx="12" cy="12" r="10" mask="url(#donutHole)"/>\n  </g>\n</svg>\n'
                 }),
-                Q = new A({
+                $ = new M({
                     name: "ui-components:close",
                     svgstr: '<svg viewBox="0 0 24 24" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon-none jp-icon-selectable-inverse jp-icon3-hover" fill="none">\n    <circle cx="12" cy="12" r="11"/>\n  </g>\n\n  <g class="jp-icon3 jp-icon-selectable jp-icon-accent2-hover" fill="#616161">\n    <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>\n  </g>\n\n  <g class="jp-icon-none jp-icon-busy" fill="none">\n    <circle cx="12" cy="12" r="7"/>\n  </g>\n</svg>\n'
                 }),
-                $ = new A({
+                J = new M({
                     name: "ui-components:code",
                     svgstr: '<svg width="22" height="22" viewBox="0 0 28 28" xmlns="http://www.w3.org/2000/svg">\n\t<g class="jp-icon3" fill="#616161">\n\t\t<path d="M11.4 18.6L6.8 14L11.4 9.4L10 8L4 14L10 20L11.4 18.6ZM16.6 18.6L21.2 14L16.6 9.4L18 8L24 14L18 20L16.6 18.6V18.6Z"/>\n\t</g>\n</svg>\n'
                 }),
-                J = new A({
+                ee = new M({
                     name: "ui-components:console",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 200 200">\n  <g class="jp-console-icon-background-color jp-icon-selectable" fill="#0288D1">\n    <path d="M20 19.8h160v159.9H20z"/>\n  </g>\n  <g class="jp-console-icon-color jp-icon-selectable-inverse" fill="#fff">\n    <path d="M105 127.3h40v12.8h-40zM51.1 77L74 99.9l-23.3 23.3 10.5 10.5 23.3-23.3L95 99.9 84.5 89.4 61.6 66.5z"/>\n  </g>\n</svg>\n'
                 }),
-                ee = new A({
+                te = new M({
                     name: "ui-components:copy",
                     svgstr: '<svg viewBox="0 0 18 18" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M11.9,1H3.2C2.4,1,1.7,1.7,1.7,2.5v10.2h1.5V2.5h8.7V1z M14.1,3.9h-8c-0.8,0-1.5,0.7-1.5,1.5v10.2c0,0.8,0.7,1.5,1.5,1.5h8 c0.8,0,1.5-0.7,1.5-1.5V5.4C15.5,4.6,14.9,3.9,14.1,3.9z M14.1,15.5h-8V5.4h8V15.5z"/>\n  </g>\n</svg>\n'
                 }),
-                te = new A({
+                ne = new M({
                     name: "ui-components:copyright",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24" viewBox="0 0 24 24" width="24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M11.88,9.14c1.28,0.06,1.61,1.15,1.63,1.66h1.79c-0.08-1.98-1.49-3.19-3.45-3.19C9.64,7.61,8,9,8,12.14 c0,1.94,0.93,4.24,3.84,4.24c2.22,0,3.41-1.65,3.44-2.95h-1.79c-0.03,0.59-0.45,1.38-1.63,1.44C10.55,14.83,10,13.81,10,12.14 C10,9.25,11.28,9.16,11.88,9.14z M12,2C6.48,2,2,6.48,2,12s4.48,10,10,10s10-4.48,10-10S17.52,2,12,2z M12,20c-4.41,0-8-3.59-8-8 s3.59-8,8-8s8,3.59,8,8S16.41,20,12,20z"/>\n  </g>\n</svg>\n'
                 }),
-                ne = new A({
+                ce = new M({
                     name: "ui-components:cut",
                     svgstr: '<svg viewBox="0 0 24 24" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M9.64 7.64c.23-.5.36-1.05.36-1.64 0-2.21-1.79-4-4-4S2 3.79 2 6s1.79 4 4 4c.59 0 1.14-.13 1.64-.36L10 12l-2.36 2.36C7.14 14.13 6.59 14 6 14c-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4c0-.59-.13-1.14-.36-1.64L12 14l7 7h3v-1L9.64 7.64zM6 8c-1.1 0-2-.89-2-2s.9-2 2-2 2 .89 2 2-.9 2-2 2zm0 12c-1.1 0-2-.89-2-2s.9-2 2-2 2 .89 2 2-.9 2-2 2zm6-7.5c-.28 0-.5-.22-.5-.5s.22-.5.5-.5.5.22.5.5-.22.5-.5.5zM19 3l-6 6 2 2 7-7V3z"/>\n  </g>\n</svg>\n'
                 }),
-                ce = new A({
+                oe = new M({
                     name: "ui-components:delete",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="16px" height="16px">\n    <path d="M0 0h24v24H0z" fill="none" />\n    <path class="jp-icon3" fill="#626262" d="M6 19c0 1.1.9 2 2 2h8c1.1 0 2-.9 2-2V7H6v12zM19 4h-3.5l-1-1h-5l-1 1H5v2h14V4z" />\n</svg>\n'
                 }),
-                oe = new A({
+                ae = new M({
                     name: "ui-components:download",
                     svgstr: '<svg viewBox="0 0 24 24" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/>\n  </g>\n</svg>\n'
                 }),
-                ae = new A({
+                re = new M({
                     name: "ui-components:duplicate",
                     svgstr: '<svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">\n<path class="jp-icon3" fill-rule="evenodd" clip-rule="evenodd" d="M2.79998 0.875H8.89582C9.20061 0.875 9.44998 1.13914 9.44998 1.46198C9.44998 1.78482 9.20061 2.04896 8.89582 2.04896H3.35415C3.04936 2.04896 2.79998 2.3131 2.79998 2.63594V9.67969C2.79998 10.0025 2.55061 10.2667 2.24582 10.2667C1.94103 10.2667 1.69165 10.0025 1.69165 9.67969V2.04896C1.69165 1.40328 2.1904 0.875 2.79998 0.875ZM5.36665 11.9V4.55H11.0833V11.9H5.36665ZM4.14165 4.14167C4.14165 3.69063 4.50728 3.325 4.95832 3.325H11.4917C11.9427 3.325 12.3083 3.69063 12.3083 4.14167V12.3083C12.3083 12.7594 11.9427 13.125 11.4917 13.125H4.95832C4.50728 13.125 4.14165 12.7594 4.14165 12.3083V4.14167Z" fill="#616161"/>\n<path class="jp-icon3" d="M9.43574 8.26507H8.36431V9.3365C8.36431 9.45435 8.26788 9.55078 8.15002 9.55078C8.03217 9.55078 7.93574 9.45435 7.93574 9.3365V8.26507H6.86431C6.74645 8.26507 6.65002 8.16864 6.65002 8.05078C6.65002 7.93292 6.74645 7.8365 6.86431 7.8365H7.93574V6.76507C7.93574 6.64721 8.03217 6.55078 8.15002 6.55078C8.26788 6.55078 8.36431 6.64721 8.36431 6.76507V7.8365H9.43574C9.5536 7.8365 9.65002 7.93292 9.65002 8.05078C9.65002 8.16864 9.5536 8.26507 9.43574 8.26507Z" fill="#616161" stroke="#616161" stroke-width="0.5"/>\n</svg>\n'
                 }),
-                re = new A({
+                se = new M({
                     name: "ui-components:edit",
                     svgstr: '<svg viewBox="0 0 24 24" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M3 17.25V21h3.75L17.81 9.94l-3.75-3.75L3 17.25zM20.71 7.04c.39-.39.39-1.02 0-1.41l-2.34-2.34c-.39-.39-1.02-.39-1.41 0l-1.83 1.83 3.75 3.75 1.83-1.83z"/>\n  </g>\n</svg>\n'
                 }),
-                se = new A({
+                le = new M({
                     name: "ui-components:ellipses",
                     svgstr: '<svg viewBox="0 0 24 24" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <circle cx="5" cy="12" r="2"/>\n    <circle cx="12" cy="12" r="2"/>\n    <circle cx="19" cy="12" r="2"/>\n  </g>\n</svg>\n'
                 }),
-                le = new A({
+                ie = new M({
                     name: "ui-components:extension",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M20.5 11H19V7c0-1.1-.9-2-2-2h-4V3.5C13 2.12 11.88 1 10.5 1S8 2.12 8 3.5V5H4c-1.1 0-1.99.9-1.99 2v3.8H3.5c1.49 0 2.7 1.21 2.7 2.7s-1.21 2.7-2.7 2.7H2V20c0 1.1.9 2 2 2h3.8v-1.5c0-1.49 1.21-2.7 2.7-2.7 1.49 0 2.7 1.21 2.7 2.7V22H17c1.1 0 2-.9 2-2v-4h1.5c1.38 0 2.5-1.12 2.5-2.5S21.88 11 20.5 11z"/>\n  </g>\n</svg>\n'
                 }),
-                ie = new A({
+                he = new M({
                     name: "ui-components:fast-forward",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M4 18l8.5-6L4 6v12zm9-12v12l8.5-6L13 6z"/>\n    </g>\n</svg>\n'
                 }),
-                he = new A({
+                pe = new M({
                     name: "ui-components:file",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <path class="jp-icon3 jp-icon-selectable" fill="#616161" d="M19.3 8.2l-5.5-5.5c-.3-.3-.7-.5-1.2-.5H3.9c-.8.1-1.6.9-1.6 1.8v14.1c0 .9.7 1.6 1.6 1.6h14.2c.9 0 1.6-.7 1.6-1.6V9.4c.1-.5-.1-.9-.4-1.2zm-5.8-3.3l3.4 3.6h-3.4V4.9zm3.9 12.7H4.7c-.1 0-.2 0-.2-.2V4.7c0-.2.1-.3.2-.3h7.2v4.4s0 .8.3 1.1c.3.3 1.1.3 1.1.3h4.3v7.2s-.1.2-.2.2z"/>\n</svg>\n'
                 }),
-                pe = new A({
+                ue = new M({
                     name: "ui-components:file-upload",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M9 16h6v-6h4l-7-7-7 7h4zm-4 2h14v2H5z"/>\n  </g>\n</svg>\n'
                 }),
-                ue = new A({
+                ve = new M({
                     name: "ui-components:filter-list",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M10 18h4v-2h-4v2zM3 6v2h18V6H3zm3 7h12v-2H6v2z"/>\n  </g>\n</svg>\n'
                 }),
-                ve = new A({
+                de = new M({
                     name: "ui-components:folder-favorite",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000">\n  <path d="M0 0h24v24H0V0z" fill="none"/><path class="jp-icon3 jp-icon-selectable" fill="#616161" d="M20 6h-8l-2-2H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V8c0-1.1-.9-2-2-2zm-2.06 11L15 15.28 12.06 17l.78-3.33-2.59-2.24 3.41-.29L15 8l1.34 3.14 3.41.29-2.59 2.24.78 3.33z"/>\n</svg>\n'
                 }),
-                de = new A({
+                me = new M({
                     name: "ui-components:folder",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-icon-selectable" fill="#616161" d="M10 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V8c0-1.1-.9-2-2-2h-8l-2-2z"/>\n</svg>\n'
                 }),
-                me = new A({
+                fe = new M({
                     name: "ui-components:home",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000">\n  <path d="M0 0h24v24H0z" fill="none"/><path class="jp-icon3 jp-icon-selectable" fill="#616161" d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/>\n</svg>\n'
                 }),
-                fe = new A({
+                Ee = new M({
                     name: "ui-components:html5",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 512 512">\n  <path class="jp-icon0 jp-icon-selectable" fill="#000" d="M108.4 0h23v22.8h21.2V0h23v69h-23V46h-21v23h-23.2M206 23h-20.3V0h63.7v23H229v46h-23m53.5-69h24.1l14.8 24.3L313.2 0h24.1v69h-23V34.8l-16.1 24.8-16.1-24.8V69h-22.6m89.2-69h23v46.2h32.6V69h-55.6"/>\n  <path class="jp-icon-selectable" fill="#e44d26" d="M107.6 471l-33-370.4h362.8l-33 370.2L255.7 512"/>\n  <path class="jp-icon-selectable" fill="#f16529" d="M256 480.5V131h148.3L376 447"/>\n  <path class="jp-icon-selectable-inverse" fill="#ebebeb" d="M142 176.3h114v45.4h-64.2l4.2 46.5h60v45.3H154.4m2 22.8H202l3.2 36.3 50.8 13.6v47.4l-93.2-26"/>\n  <path class="jp-icon-selectable-inverse" fill="#fff" d="M369.6 176.3H255.8v45.4h109.6m-4.1 46.5H255.8v45.4h56l-5.3 59-50.7 13.6v47.2l93-25.8"/>\n</svg>\n'
                 }),
-                Ee = new A({
+                ze = new M({
                     name: "ui-components:image",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <path class="jp-icon-brand4 jp-icon-selectable-inverse" fill="#FFF" d="M2.2 2.2h17.5v17.5H2.2z"/>\n  <path class="jp-icon-brand0 jp-icon-selectable" fill="#3F51B5" d="M2.2 2.2v17.5h17.5l.1-17.5H2.2zm12.1 2.2c1.2 0 2.2 1 2.2 2.2s-1 2.2-2.2 2.2-2.2-1-2.2-2.2 1-2.2 2.2-2.2zM4.4 17.6l3.3-8.8 3.3 6.6 2.2-3.2 4.4 5.4H4.4z"/>\n</svg>\n'
                 }),
-                ze = new A({
+                ge = new M({
                     name: "ui-components:inspector",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <path class="jp-inspector-icon-color jp-icon-selectable" fill="#616161" d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm-5 14H4v-4h11v4zm0-5H4V9h11v4zm5 5h-4V9h4v9z"/>\n</svg>\n'
                 }),
-                ge = new A({
+                _e = new M({
                     name: "ui-components:json",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <g class="jp-json-icon-color jp-icon-selectable" fill="#F9A825">\n    <path d="M20.2 11.8c-1.6 0-1.7.5-1.7 1 0 .4.1.9.1 1.3.1.5.1.9.1 1.3 0 1.7-1.4 2.3-3.5 2.3h-.9v-1.9h.5c1.1 0 1.4 0 1.4-.8 0-.3 0-.6-.1-1 0-.4-.1-.8-.1-1.2 0-1.3 0-1.8 1.3-2-1.3-.2-1.3-.7-1.3-2 0-.4.1-.8.1-1.2.1-.4.1-.7.1-1 0-.8-.4-.7-1.4-.8h-.5V4.1h.9c2.2 0 3.5.7 3.5 2.3 0 .4-.1.9-.1 1.3-.1.5-.1.9-.1 1.3 0 .5.2 1 1.7 1v1.8zM1.8 10.1c1.6 0 1.7-.5 1.7-1 0-.4-.1-.9-.1-1.3-.1-.5-.1-.9-.1-1.3 0-1.6 1.4-2.3 3.5-2.3h.9v1.9h-.5c-1 0-1.4 0-1.4.8 0 .3 0 .6.1 1 0 .2.1.6.1 1 0 1.3 0 1.8-1.3 2C6 11.2 6 11.7 6 13c0 .4-.1.8-.1 1.2-.1.3-.1.7-.1 1 0 .8.3.8 1.4.8h.5v1.9h-.9c-2.1 0-3.5-.6-3.5-2.3 0-.4.1-.9.1-1.3.1-.5.1-.9.1-1.3 0-.5-.2-1-1.7-1v-1.9z"/>\n    <circle cx="11" cy="13.8" r="2.1"/>\n    <circle cx="11" cy="8.2" r="2.1"/>\n  </g>\n</svg>\n'
                 }),
-                _e = new A({
+                Le = new M({
                     name: "ui-components:julia",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 325 300">\n  <g class="jp-brand0 jp-icon-selectable" fill="#cb3c33">\n    <path d="M 150.898438 225 C 150.898438 266.421875 117.320312 300 75.898438 300 C 34.476562 300 0.898438 266.421875 0.898438 225 C 0.898438 183.578125 34.476562 150 75.898438 150 C 117.320312 150 150.898438 183.578125 150.898438 225"/>\n  </g>\n  <g class="jp-brand0 jp-icon-selectable" fill="#389826">\n    <path d="M 237.5 75 C 237.5 116.421875 203.921875 150 162.5 150 C 121.078125 150 87.5 116.421875 87.5 75 C 87.5 33.578125 121.078125 0 162.5 0 C 203.921875 0 237.5 33.578125 237.5 75"/>\n  </g>\n  <g class="jp-brand0 jp-icon-selectable" fill="#9558b2">\n    <path d="M 324.101562 225 C 324.101562 266.421875 290.523438 300 249.101562 300 C 207.679688 300 174.101562 266.421875 174.101562 225 C 174.101562 183.578125 207.679688 150 249.101562 150 C 290.523438 150 324.101562 183.578125 324.101562 225"/>\n  </g>\n</svg>\n'
                 }),
-                Le = new A({
+                Ce = new M({
                     name: "ui-components:jupyter-favicon",
                     svgstr: '<svg width="152" height="165" viewBox="0 0 152 165" version="1.1" xmlns="http://www.w3.org/2000/svg">\n   <g class="jp-jupyter-icon-color" fill="#F37726">\n    <path transform="translate(0.078947, 110.582927)" d="M75.9422842,29.5804561 C43.3023947,29.5804561 14.7967832,17.6534634 0,0 C5.51083211,15.8406829 15.7815389,29.5667732 29.3904947,39.2784171 C42.9997,48.9898537 59.2737,54.2067805 75.9605789,54.2067805 C92.6474579,54.2067805 108.921458,48.9898537 122.530663,39.2784171 C136.139453,29.5667732 146.410284,15.8406829 151.921158,0 C137.087868,17.6534634 108.582589,29.5804561 75.9422842,29.5804561 L75.9422842,29.5804561 Z" />\n    <path transform="translate(0.037368, 0.704878)" d="M75.9784579,24.6264073 C108.618763,24.6264073 137.124458,36.5534415 151.921158,54.2067805 C146.410284,38.366222 136.139453,24.6401317 122.530663,14.9284878 C108.921458,5.2168439 92.6474579,0 75.9605789,0 C59.2737,0 42.9997,5.2168439 29.3904947,14.9284878 C15.7815389,24.6401317 5.51083211,38.366222 0,54.2067805 C14.8330816,36.5899293 43.3385684,24.6264073 75.9784579,24.6264073 L75.9784579,24.6264073 Z" />\n  </g>\n</svg>\n'
                 }),
-                Ce = new A({
+                Ae = new M({
                     name: "ui-components:jupyter",
                     svgstr: '<svg width="39" height="51" viewBox="0 0 39 51" xmlns="http://www.w3.org/2000/svg">\n  <g transform="translate(-1638 -2281)">\n     <g class="jp-jupyter-icon-color" fill="#F37726">\n      <path transform="translate(1639.74 2311.98)" d="M 18.2646 7.13411C 10.4145 7.13411 3.55872 4.2576 0 0C 1.32539 3.8204 3.79556 7.13081 7.0686 9.47303C 10.3417 11.8152 14.2557 13.0734 18.269 13.0734C 22.2823 13.0734 26.1963 11.8152 29.4694 9.47303C 32.7424 7.13081 35.2126 3.8204 36.538 0C 32.9705 4.2576 26.1148 7.13411 18.2646 7.13411Z"/>\n      <path transform="translate(1639.73 2285.48)" d="M 18.2733 5.93931C 26.1235 5.93931 32.9793 8.81583 36.538 13.0734C 35.2126 9.25303 32.7424 5.94262 29.4694 3.6004C 26.1963 1.25818 22.2823 0 18.269 0C 14.2557 0 10.3417 1.25818 7.0686 3.6004C 3.79556 5.94262 1.32539 9.25303 0 13.0734C 3.56745 8.82463 10.4232 5.93931 18.2733 5.93931Z"/>\n    </g>\n    <g class="jp-icon3" fill="#616161">\n      <path transform="translate(1669.3 2281.31)" d="M 5.89353 2.844C 5.91889 3.43165 5.77085 4.01367 5.46815 4.51645C 5.16545 5.01922 4.72168 5.42015 4.19299 5.66851C 3.6643 5.91688 3.07444 6.00151 2.49805 5.91171C 1.92166 5.8219 1.38463 5.5617 0.954898 5.16401C 0.52517 4.76633 0.222056 4.24903 0.0839037 3.67757C -0.0542483 3.10611 -0.02123 2.50617 0.178781 1.95364C 0.378793 1.4011 0.736809 0.920817 1.20754 0.573538C 1.67826 0.226259 2.24055 0.0275919 2.82326 0.00267229C 3.60389 -0.0307115 4.36573 0.249789 4.94142 0.782551C 5.51711 1.31531 5.85956 2.05676 5.89353 2.844Z"/>\n      <path transform="translate(1639.8 2323.81)" d="M 7.42789 3.58338C 7.46008 4.3243 7.27355 5.05819 6.89193 5.69213C 6.51031 6.32607 5.95075 6.83156 5.28411 7.1446C 4.61747 7.45763 3.87371 7.56414 3.14702 7.45063C 2.42032 7.33712 1.74336 7.0087 1.20184 6.50695C 0.660328 6.0052 0.27861 5.35268 0.105017 4.63202C -0.0685757 3.91135 -0.0262361 3.15494 0.226675 2.45856C 0.479587 1.76217 0.931697 1.15713 1.52576 0.720033C 2.11983 0.282935 2.82914 0.0334395 3.56389 0.00313344C 4.54667 -0.0374033 5.50529 0.316706 6.22961 0.987835C 6.95393 1.65896 7.38484 2.59235 7.42789 3.58338L 7.42789 3.58338Z"/>\n      <path transform="translate(1638.36 2286.06)" d="M 2.27471 4.39629C 1.84363 4.41508 1.41671 4.30445 1.04799 4.07843C 0.679268 3.8524 0.385328 3.52114 0.203371 3.12656C 0.0214136 2.73198 -0.0403798 2.29183 0.0258116 1.86181C 0.0920031 1.4318 0.283204 1.03126 0.575213 0.710883C 0.867222 0.39051 1.24691 0.164708 1.66622 0.0620592C 2.08553 -0.0405897 2.52561 -0.0154714 2.93076 0.134235C 3.33591 0.283941 3.68792 0.551505 3.94222 0.90306C 4.19652 1.25462 4.34169 1.67436 4.35935 2.10916C 4.38299 2.69107 4.17678 3.25869 3.78597 3.68746C 3.39516 4.11624 2.85166 4.37116 2.27471 4.39629L 2.27471 4.39629Z"/>\n    </g>\n  </g>>\n</svg>\n'
                 }),
-                Ae = new A({
+                Me = new M({
                     name: "ui-components:jupyterlab-wordmark",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="200" viewBox="0 0 1860.8 475">\n  <g class="jp-icon2" fill="#4E4E4E" transform="translate(480.136401, 64.271493)">\n    <g transform="translate(0.000000, 58.875566)">\n      <g transform="translate(0.087603, 0.140294)">\n        <path d="M-426.9,169.8c0,48.7-3.7,64.7-13.6,76.4c-10.8,10-25,15.5-39.7,15.5l3.7,29 c22.8,0.3,44.8-7.9,61.9-23.1c17.8-18.5,24-44.1,24-83.3V0H-427v170.1L-426.9,169.8L-426.9,169.8z"/>\n      </g>\n    </g>\n    <g transform="translate(155.045296, 56.837104)">\n      <g transform="translate(1.562453, 1.799842)">\n        <path d="M-312,148c0,21,0,39.5,1.7,55.4h-31.8l-2.1-33.3h-0.8c-6.7,11.6-16.4,21.3-28,27.9 c-11.6,6.6-24.8,10-38.2,9.8c-31.4,0-69-17.7-69-89V0h36.4v112.7c0,38.7,11.6,64.7,44.6,64.7c10.3-0.2,20.4-3.5,28.9-9.4 c8.5-5.9,15.1-14.3,18.9-23.9c2.2-6.1,3.3-12.5,3.3-18.9V0.2h36.4V148H-312L-312,148z"/>\n      </g>\n    </g>\n    <g transform="translate(390.013322, 53.479638)">\n      <g transform="translate(1.706458, 0.231425)">\n        <path d="M-478.6,71.4c0-26-0.8-47-1.7-66.7h32.7l1.7,34.8h0.8c7.1-12.5,17.5-22.8,30.1-29.7 c12.5-7,26.7-10.3,41-9.8c48.3,0,84.7,41.7,84.7,103.3c0,73.1-43.7,109.2-91,109.2c-12.1,0.5-24.2-2.2-35-7.8 c-10.8-5.6-19.9-13.9-26.6-24.2h-0.8V291h-36v-220L-478.6,71.4L-478.6,71.4z M-442.6,125.6c0.1,5.1,0.6,10.1,1.7,15.1 c3,12.3,9.9,23.3,19.8,31.1c9.9,7.8,22.1,12.1,34.7,12.1c38.5,0,60.7-31.9,60.7-78.5c0-40.7-21.1-75.6-59.5-75.6 c-12.9,0.4-25.3,5.1-35.3,13.4c-9.9,8.3-16.9,19.7-19.6,32.4c-1.5,4.9-2.3,10-2.5,15.1V125.6L-442.6,125.6L-442.6,125.6z"/>\n      </g>\n    </g>\n    <g transform="translate(606.740726, 56.837104)">\n      <g transform="translate(0.751226, 1.989299)">\n        <path d="M-440.8,0l43.7,120.1c4.5,13.4,9.5,29.4,12.8,41.7h0.8c3.7-12.2,7.9-27.7,12.8-42.4 l39.7-119.2h38.5L-346.9,145c-26,69.7-43.7,105.4-68.6,127.2c-12.5,11.7-27.9,20-44.6,23.9l-9.1-31.1 c11.7-3.9,22.5-10.1,31.8-18.1c13.2-11.1,23.7-25.2,30.6-41.2c1.5-2.8,2.5-5.7,2.9-8.8c-0.3-3.3-1.2-6.6-2.5-9.7L-480.2,0.1 h39.7L-440.8,0L-440.8,0z"/>\n      </g>\n    </g>\n    <g transform="translate(822.748104, 0.000000)">\n      <g transform="translate(1.464050, 0.378914)">\n        <path d="M-413.7,0v58.3h52v28.2h-52V196c0,25,7,39.5,27.3,39.5c7.1,0.1,14.2-0.7,21.1-2.5 l1.7,27.7c-10.3,3.7-21.3,5.4-32.2,5c-7.3,0.4-14.6-0.7-21.3-3.4c-6.8-2.7-12.9-6.8-17.9-12.1c-10.3-10.9-14.1-29-14.1-52.9 V86.5h-31V58.3h31V9.6L-413.7,0L-413.7,0z"/>\n      </g>\n    </g>\n    <g transform="translate(974.433286, 53.479638)">\n      <g transform="translate(0.990034, 0.610339)">\n        <path d="M-445.8,113c0.8,50,32.2,70.6,68.6,70.6c19,0.6,37.9-3,55.3-10.5l6.2,26.4 c-20.9,8.9-43.5,13.1-66.2,12.6c-61.5,0-98.3-41.2-98.3-102.5C-480.2,48.2-444.7,0-386.5,0c65.2,0,82.7,58.3,82.7,95.7 c-0.1,5.8-0.5,11.5-1.2,17.2h-140.6H-445.8L-445.8,113z M-339.2,86.6c0.4-23.5-9.5-60.1-50.4-60.1 c-36.8,0-52.8,34.4-55.7,60.1H-339.2L-339.2,86.6L-339.2,86.6z"/>\n      </g>\n    </g>\n    <g transform="translate(1201.961058, 53.479638)">\n      <g transform="translate(1.179640, 0.705068)">\n        <path d="M-478.6,68c0-23.9-0.4-44.5-1.7-63.4h31.8l1.2,39.9h1.7c9.1-27.3,31-44.5,55.3-44.5 c3.5-0.1,7,0.4,10.3,1.2v34.8c-4.1-0.9-8.2-1.3-12.4-1.2c-25.6,0-43.7,19.7-48.7,47.4c-1,5.7-1.6,11.5-1.7,17.2v108.3h-36V68 L-478.6,68z"/>\n      </g>\n    </g>\n  </g>\n\n  <g class="jp-icon-warn0" fill="#F37726">\n    <path d="M1352.3,326.2h37V28h-37V326.2z M1604.8,326.2c-2.5-13.9-3.4-31.1-3.4-48.7v-76 c0-40.7-15.1-83.1-77.3-83.1c-25.6,0-50,7.1-66.8,18.1l8.4,24.4c14.3-9.2,34-15.1,53-15.1c41.6,0,46.2,30.2,46.2,47v4.2 c-78.6-0.4-122.3,26.5-122.3,75.6c0,29.4,21,58.4,62.2,58.4c29,0,50.9-14.3,62.2-30.2h1.3l2.9,25.6H1604.8z M1565.7,257.7 c0,3.8-0.8,8-2.1,11.8c-5.9,17.2-22.7,34-49.2,34c-18.9,0-34.9-11.3-34.9-35.3c0-39.5,45.8-46.6,86.2-45.8V257.7z M1698.5,326.2 l1.7-33.6h1.3c15.1,26.9,38.7,38.2,68.1,38.2c45.4,0,91.2-36.1,91.2-108.8c0.4-61.7-35.3-103.7-85.7-103.7 c-32.8,0-56.3,14.7-69.3,37.4h-0.8V28h-36.6v245.7c0,18.1-0.8,38.6-1.7,52.5H1698.5z M1704.8,208.2c0-5.9,1.3-10.9,2.1-15.1 c7.6-28.1,31.1-45.4,56.3-45.4c39.5,0,60.5,34.9,60.5,75.6c0,46.6-23.1,78.1-61.8,78.1c-26.9,0-48.3-17.6-55.5-43.3 c-0.8-4.2-1.7-8.8-1.7-13.4V208.2z"/>\n  </g>\n</svg>\n'
                 }),
-                Me = new A({
+                Te = new M({
                     name: "ui-components:kernel",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n    <path class="jp-icon2" fill="#616161" d="M15 9H9v6h6V9zm-2 4h-2v-2h2v2zm8-2V9h-2V7c0-1.1-.9-2-2-2h-2V3h-2v2h-2V3H9v2H7c-1.1 0-2 .9-2 2v2H3v2h2v2H3v2h2v2c0 1.1.9 2 2 2h2v2h2v-2h2v2h2v-2h2c1.1 0 2-.9 2-2v-2h2v-2h-2v-2h2zm-4 6H7V7h10v10z"/>\n</svg>\n'
                 }),
-                Te = new A({
+                ye = new M({
                     name: "ui-components:keyboard",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-icon-selectable" fill="#616161" d="M20 5H4c-1.1 0-1.99.9-1.99 2L2 17c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V7c0-1.1-.9-2-2-2zm-9 3h2v2h-2V8zm0 3h2v2h-2v-2zM8 8h2v2H8V8zm0 3h2v2H8v-2zm-1 2H5v-2h2v2zm0-3H5V8h2v2zm9 7H8v-2h8v2zm0-4h-2v-2h2v2zm0-3h-2V8h2v2zm3 3h-2v-2h2v2zm0-3h-2V8h2v2z"/>\n</svg>\n'
                 }),
-                ye = new A({
+                Oe = new M({
                     name: "ui-components:launch",
                     svgstr: '<svg viewBox="0 0 32 32" width="32" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3 jp-icon-selectable" fill="#616161">\n    <path d="M26,28H6a2.0027,2.0027,0,0,1-2-2V6A2.0027,2.0027,0,0,1,6,4H16V6H6V26H26V16h2V26A2.0027,2.0027,0,0,1,26,28Z"/>\n    <polygon points="20 2 20 4 26.586 4 18 12.586 19.414 14 28 5.414 28 12 30 12 30 2 20 2"/>\n  </g>\n</svg>\n'
                 }),
-                Oe = new A({
+                He = new M({
                     name: "ui-components:launcher",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-icon-selectable" fill="#616161" d="M19 19H5V5h7V3H5a2 2 0 00-2 2v14a2 2 0 002 2h14c1.1 0 2-.9 2-2v-7h-2v7zM14 3v2h3.59l-9.83 9.83 1.41 1.41L19 6.41V10h2V3h-7z"/>\n</svg>\n'
                 }),
-                He = new A({
+                Re = new M({
                     name: "ui-components:line-form",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n    <path fill="white" d="M5.88 4.12L13.76 12l-7.88 7.88L8 22l10-10L8 2z"/>\n</svg>\n'
                 }),
-                Re = new A({
+                Ne = new M({
                     name: "ui-components:link",
                     svgstr: '<svg viewBox="0 0 24 24" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76 0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71 0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71 0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76 0 5-2.24 5-5s-2.24-5-5-5z"/>\n  </g>\n</svg>\n'
                 }),
-                Ne = new A({
+                Ie = new M({
                     name: "ui-components:list",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n    <path class="jp-icon2 jp-icon-selectable" fill="#616161" d="M19 5v14H5V5h14m1.1-2H3.9c-.5 0-.9.4-.9.9v16.2c0 .4.4.9.9.9h16.2c.4 0 .9-.5.9-.9V3.9c0-.5-.5-.9-.9-.9zM11 7h6v2h-6V7zm0 4h6v2h-6v-2zm0 4h6v2h-6zM7 7h2v2H7zm0 4h2v2H7zm0 4h2v2H7z"/>\n</svg>'
                 }),
-                Ie = new A({
+                Ve = new M({
                     name: "ui-components:listings-info",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 50.978 50.978" style="enable-background:new 0 0 50.978 50.978;" xml:space="preserve">\n\t<g>\n\t\t<path style="fill:#010002;" d="M43.52,7.458C38.711,2.648,32.307,0,25.489,0C18.67,0,12.266,2.648,7.458,7.458\n\t\t\tc-9.943,9.941-9.943,26.119,0,36.062c4.809,4.809,11.212,7.456,18.031,7.458c0,0,0.001,0,0.002,0\n\t\t\tc6.816,0,13.221-2.648,18.029-7.458c4.809-4.809,7.457-11.212,7.457-18.03C50.977,18.67,48.328,12.266,43.52,7.458z\n\t\t\t M42.106,42.105c-4.432,4.431-10.332,6.872-16.615,6.872h-0.002c-6.285-0.001-12.187-2.441-16.617-6.872\n\t\t\tc-9.162-9.163-9.162-24.071,0-33.233C13.303,4.44,19.204,2,25.489,2c6.284,0,12.186,2.44,16.617,6.872\n\t\t\tc4.431,4.431,6.871,10.332,6.871,16.617C48.977,31.772,46.536,37.675,42.106,42.105z"/>\n\t\t<path style="fill:#010002;" d="M23.578,32.218c-0.023-1.734,0.143-3.059,0.496-3.972c0.353-0.913,1.11-1.997,2.272-3.253\n\t\t\tc0.468-0.536,0.923-1.062,1.367-1.575c0.626-0.753,1.104-1.478,1.436-2.175c0.331-0.707,0.495-1.541,0.495-2.5\n\t\t\tc0-1.096-0.26-2.088-0.779-2.979c-0.565-0.879-1.501-1.336-2.806-1.369c-1.802,0.057-2.985,0.667-3.55,1.832\n\t\t\tc-0.301,0.535-0.503,1.141-0.607,1.814c-0.139,0.707-0.207,1.432-0.207,2.174h-2.937c-0.091-2.208,0.407-4.114,1.493-5.719\n\t\t\tc1.062-1.64,2.855-2.481,5.378-2.527c2.16,0.023,3.874,0.608,5.141,1.758c1.278,1.16,1.929,2.764,1.95,4.811\n\t\t\tc0,1.142-0.137,2.111-0.41,2.911c-0.309,0.845-0.731,1.593-1.268,2.243c-0.492,0.65-1.068,1.318-1.73,2.002\n\t\t\tc-0.65,0.697-1.313,1.479-1.987,2.346c-0.239,0.377-0.429,0.777-0.565,1.199c-0.16,0.959-0.217,1.951-0.171,2.979\n\t\t\tC26.589,32.218,23.578,32.218,23.578,32.218z M23.578,38.22v-3.484h3.076v3.484H23.578z"/>\n\t</g>\n</svg>\n'
                 }),
-                Ve = new A({
+                Se = new M({
                     name: "ui-components:markdown",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <path class="jp-icon-contrast0 jp-icon-selectable" fill="#7B1FA2" d="M5 14.9h12l-6.1 6zm9.4-6.8c0-1.3-.1-2.9-.1-4.5-.4 1.4-.9 2.9-1.3 4.3l-1.3 4.3h-2L8.5 7.9c-.4-1.3-.7-2.9-1-4.3-.1 1.6-.1 3.2-.2 4.6L7 12.4H4.8l.7-11h3.3L10 5c.4 1.2.7 2.7 1 3.9.3-1.2.7-2.6 1-3.9l1.2-3.7h3.3l.6 11h-2.4l-.3-4.2z"/>\n</svg>\n'
                 }),
-                Se = new A({
+                be = new M({
                     name: "ui-components:move-down",
                     svgstr: '<svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">\n<path class="jp-icon3" d="M12.471 7.52899C12.7632 7.23684 12.7632 6.76316 12.471 6.47101V6.47101C12.179 6.17905 11.7057 6.17884 11.4135 6.47054L7.75 10.1275V1.75C7.75 1.33579 7.41421 1 7 1V1C6.58579 1 6.25 1.33579 6.25 1.75V10.1275L2.59726 6.46822C2.30338 6.17381 1.82641 6.17359 1.53226 6.46774V6.46774C1.2383 6.7617 1.2383 7.2383 1.53226 7.53226L6.29289 12.2929C6.68342 12.6834 7.31658 12.6834 7.70711 12.2929L12.471 7.52899Z" fill="#616161"/>\n</svg>\n'
                 }),
-                be = new A({
+                we = new M({
                     name: "ui-components:move-up",
                     svgstr: '<svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">\n<path class="jp-icon3" d="M1.52899 6.47101C1.23684 6.76316 1.23684 7.23684 1.52899 7.52899V7.52899C1.82095 7.82095 2.29426 7.82116 2.58649 7.52946L6.25 3.8725V12.25C6.25 12.6642 6.58579 13 7 13V13C7.41421 13 7.75 12.6642 7.75 12.25V3.8725L11.4027 7.53178C11.6966 7.82619 12.1736 7.82641 12.4677 7.53226V7.53226C12.7617 7.2383 12.7617 6.7617 12.4677 6.46774L7.70711 1.70711C7.31658 1.31658 6.68342 1.31658 6.29289 1.70711L1.52899 6.47101Z" fill="#616161"/>\n</svg>\n'
                 }),
-                we = new A({
+                Pe = new M({
                     name: "ui-components:new-folder",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M20 6h-8l-2-2H4c-1.11 0-1.99.89-1.99 2L2 18c0 1.11.89 2 2 2h16c1.11 0 2-.89 2-2V8c0-1.11-.89-2-2-2zm-1 8h-3v3h-2v-3h-3v-2h3V9h2v3h3v2z"/>\n  </g>\n</svg>\n'
                 }),
-                Pe = new A({
+                De = new M({
                     name: "ui-components:not-trusted",
                     svgstr: '<svg fill="none" xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 25 25">\n    <path class="jp-icon2" stroke="#333333" stroke-width="2" transform="translate(3 3)" d="M1.86094 11.4409C0.826448 8.77027 0.863779 6.05764 1.24907 4.19932C2.48206 3.93347 4.08068 3.40347 5.60102 2.8449C7.23549 2.2444 8.85666 1.5815 9.9876 1.09539C11.0597 1.58341 12.6094 2.2444 14.218 2.84339C15.7503 3.41394 17.3995 3.95258 18.7539 4.21385C19.1364 6.07177 19.1709 8.77722 18.139 11.4409C17.0303 14.3032 14.6668 17.1844 9.99999 18.9354C5.33319 17.1844 2.96968 14.3032 1.86094 11.4409Z"/>\n    <path class="jp-icon2" stroke="#333333" stroke-width="2" transform="translate(9.31592 9.32031)" d="M7.36842 0L0 7.36479"/>\n    <path class="jp-icon2" stroke="#333333" stroke-width="2" transform="translate(9.31592 16.6836) scale(1 -1)" d="M7.36842 0L0 7.36479"/>\n</svg>\n'
                 }),
-                De = new A({
+                xe = new M({
                     name: "ui-components:notebook",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <g class="jp-notebook-icon-color jp-icon-selectable" fill="#EF6C00">\n    <path d="M18.7 3.3v15.4H3.3V3.3h15.4m1.5-1.5H1.8v18.3h18.3l.1-18.3z"/>\n    <path d="M16.5 16.5l-5.4-4.3-5.6 4.3v-11h11z"/>\n  </g>\n</svg>\n'
                 }),
-                xe = new A({
+                Be = new M({
                     name: "ui-components:numbering",
                     svgstr: '<svg width="22" height="22" viewBox="0 0 28 28" xmlns="http://www.w3.org/2000/svg">\n\t<g class="jp-icon3" fill="#616161">\n\t\t<path d="M4 19H6V19.5H5V20.5H6V21H4V22H7V18H4V19ZM5 10H6V6H4V7H5V10ZM4 13H5.8L4 15.1V16H7V15H5.2L7 12.9V12H4V13ZM9 7V9H23V7H9ZM9 21H23V19H9V21ZM9 15H23V13H9V15Z"/>\n\t</g>\n</svg>\n'
                 }),
-                Be = new A({
+                ke = new M({
                     name: "ui-components:offline-bolt",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="16">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M12 2.02c-5.51 0-9.98 4.47-9.98 9.98s4.47 9.98 9.98 9.98 9.98-4.47 9.98-9.98S17.51 2.02 12 2.02zM11.48 20v-6.26H8L13 4v6.26h3.35L11.48 20z"/>\n  </g>\n</svg>\n'
                 }),
-                ke = new A({
+                Ue = new M({
                     name: "ui-components:palette",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M18 13V20H4V6H9.02C9.07 5.29 9.24 4.62 9.5 4H4C2.9 4 2 4.9 2 6V20C2 21.1 2.9 22 4 22H18C19.1 22 20 21.1 20 20V15L18 13ZM19.3 8.89C19.74 8.19 20 7.38 20 6.5C20 4.01 17.99 2 15.5 2C13.01 2 11 4.01 11 6.5C11 8.99 13.01 11 15.49 11C16.37 11 17.19 10.74 17.88 10.3L21 13.42L22.42 12L19.3 8.89ZM15.5 9C14.12 9 13 7.88 13 6.5C13 5.12 14.12 4 15.5 4C16.88 4 18 5.12 18 6.5C18 7.88 16.88 9 15.5 9Z"/>\n    <path fill-rule="evenodd" clip-rule="evenodd" d="M4 6H9.01894C9.00639 6.16502 9 6.33176 9 6.5C9 8.81577 10.211 10.8487 12.0343 12H9V14H16V12.9811C16.5703 12.9377 17.12 12.8207 17.6396 12.6396L18 13V20H4V6ZM8 8H6V10H8V8ZM6 12H8V14H6V12ZM8 16H6V18H8V16ZM9 16H16V18H9V16Z"/>\n  </g>\n</svg>\n'
                 }),
-                Ue = new A({
+                Fe = new M({
                     name: "ui-components:paste",
                     svgstr: '<svg height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M19 2h-4.18C14.4.84 13.3 0 12 0c-1.3 0-2.4.84-2.82 2H5c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V4c0-1.1-.9-2-2-2zm-7 0c.55 0 1 .45 1 1s-.45 1-1 1-1-.45-1-1 .45-1 1-1zm7 18H5V4h2v3h10V4h2v16z"/>\n    </g>\n</svg>\n'
                 }),
-                Fe = new A({
+                Ge = new M({
                     name: "ui-components:pdf",
                     svgstr: '<svg\n   xmlns="http://www.w3.org/2000/svg" viewBox="0 0 22 22" width="16">\n    <path transform="rotate(45)" class="jp-icon-selectable" fill="#FF2A2A"\n       d="m 22.344369,-3.0163642 h 5.638604 v 1.5792433 h -3.549227 v 1.50869299 h 3.337576 V 1.6508154 h -3.337576 v 3.4352613 h -2.089377 z m -7.136444,1.5792433 v 4.9439543 h 0.74892 q 1.280761,0 1.953703,-0.6349535 0.678369,-0.6349535 0.678369,-1.8451641 0,-1.20478355 -0.672942,-1.83431011 -0.672942,-0.62952659 -1.95913,-0.62952659 z m -2.089377,-1.5792433 h 2.203343 q 1.845164,0 2.746039,0.2659207 0.906301,0.2604937 1.552108,0.8900203 0.56983,0.5481223 0.846605,1.26448006 0.276774,0.71635781 0.276774,1.62265894 0,0.9171551 -0.276774,1.6389399 -0.276775,0.7163578 -0.846605,1.26448 -0.651234,0.6295266 -1.562962,0.8954473 -0.911728,0.2604937 -2.735185,0.2604937 h -2.203343 z m -8.1458565,0 h 3.467823 q 1.5466816,0 2.3715785,0.689223 0.830324,0.6837961 0.830324,1.95370314 0,1.27533397 -0.830324,1.96455706 Q 9.9871961,2.274915 8.4405145,2.274915 H 7.0620684 V 5.0860767 H 4.9726915 Z m 2.0893769,1.5141199 v 2.26303943 h 1.155941 q 0.6078188,0 0.9388629,-0.29305547 0.3310441,-0.29848241 0.3310441,-0.84117772 0,-0.54269531 -0.3310441,-0.83575074 -0.3310441,-0.2930555 -0.9388629,-0.2930555 z"\n/>\n</svg>\n'
                 }),
-                Ge = new A({
+                je = new M({
                     name: "ui-components:python",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="-10 -10 131.16136169433594 132.38899993896484">\n  <path class="jp-icon-selectable" fill="#306998" d="M 54.918785,9.1927421e-4 C 50.335132,0.02221727 45.957846,0.41313697 42.106285,1.0946693 30.760069,3.0991731 28.700036,7.2947714 28.700035,15.032169 v 10.21875 h 26.8125 v 3.40625 h -26.8125 -10.0625 c -7.792459,0 -14.6157588,4.683717 -16.7499998,13.59375 -2.46181998,10.212966 -2.57101508,16.586023 0,27.25 1.9059283,7.937852 6.4575432,13.593748 14.2499998,13.59375 h 9.21875 v -12.25 c 0,-8.849902 7.657144,-16.656248 16.75,-16.65625 h 26.78125 c 7.454951,0 13.406253,-6.138164 13.40625,-13.625 v -25.53125 c 0,-7.2663386 -6.12998,-12.7247771 -13.40625,-13.9374997 C 64.281548,0.32794397 59.502438,-0.02037903 54.918785,9.1927421e-4 Z m -14.5,8.21875012579 c 2.769547,0 5.03125,2.2986456 5.03125,5.1249996 -2e-6,2.816336 -2.261703,5.09375 -5.03125,5.09375 -2.779476,-1e-6 -5.03125,-2.277415 -5.03125,-5.09375 -10e-7,-2.826353 2.251774,-5.1249996 5.03125,-5.1249996 z"/>\n  <path class="jp-icon-selectable" fill="#ffd43b" d="m 85.637535,28.657169 v 11.90625 c 0,9.230755 -7.825895,16.999999 -16.75,17 h -26.78125 c -7.335833,0 -13.406249,6.278483 -13.40625,13.625 v 25.531247 c 0,7.266344 6.318588,11.540324 13.40625,13.625004 8.487331,2.49561 16.626237,2.94663 26.78125,0 6.750155,-1.95439 13.406253,-5.88761 13.40625,-13.625004 V 86.500919 h -26.78125 v -3.40625 h 26.78125 13.406254 c 7.792461,0 10.696251,-5.435408 13.406241,-13.59375 2.79933,-8.398886 2.68022,-16.475776 0,-27.25 -1.92578,-7.757441 -5.60387,-13.59375 -13.406241,-13.59375 z m -15.0625,64.65625 c 2.779478,3e-6 5.03125,2.277417 5.03125,5.093747 -2e-6,2.826354 -2.251775,5.125004 -5.03125,5.125004 -2.76955,0 -5.03125,-2.29865 -5.03125,-5.125004 2e-6,-2.81633 2.261697,-5.093747 5.03125,-5.093747 z"/>\n</svg>\n'
                 }),
-                je = new A({
+                Ke = new M({
                     name: "ui-components:r-kernel",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <path class="jp-icon-contrast3 jp-icon-selectable" fill="#2196F3" d="M4.4 2.5c1.2-.1 2.9-.3 4.9-.3 2.5 0 4.1.4 5.2 1.3 1 .7 1.5 1.9 1.5 3.5 0 2-1.4 3.5-2.9 4.1 1.2.4 1.7 1.6 2.2 3 .6 1.9 1 3.9 1.3 4.6h-3.8c-.3-.4-.8-1.7-1.2-3.7s-1.2-2.6-2.6-2.6h-.9v6.4H4.4V2.5zm3.7 6.9h1.4c1.9 0 2.9-.9 2.9-2.3s-1-2.3-2.8-2.3c-.7 0-1.3 0-1.6.2v4.5h.1v-.1z"/>\n</svg>\n'
                 }),
-                Ke = new A({
+                We = new M({
                     name: "ui-components:react",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="150 150 541.9 295.3">\n  <g class="jp-icon-brand2 jp-icon-selectable" fill="#61DAFB">\n    <path d="M666.3 296.5c0-32.5-40.7-63.3-103.1-82.4 14.4-63.6 8-114.2-20.2-130.4-6.5-3.8-14.1-5.6-22.4-5.6v22.3c4.6 0 8.3.9 11.4 2.6 13.6 7.8 19.5 37.5 14.9 75.7-1.1 9.4-2.9 19.3-5.1 29.4-19.6-4.8-41-8.5-63.5-10.9-13.5-18.5-27.5-35.3-41.6-50 32.6-30.3 63.2-46.9 84-46.9V78c-27.5 0-63.5 19.6-99.9 53.6-36.4-33.8-72.4-53.2-99.9-53.2v22.3c20.7 0 51.4 16.5 84 46.6-14 14.7-28 31.4-41.3 49.9-22.6 2.4-44 6.1-63.6 11-2.3-10-4-19.7-5.2-29-4.7-38.2 1.1-67.9 14.6-75.8 3-1.8 6.9-2.6 11.5-2.6V78.5c-8.4 0-16 1.8-22.6 5.6-28.1 16.2-34.4 66.7-19.9 130.1-62.2 19.2-102.7 49.9-102.7 82.3 0 32.5 40.7 63.3 103.1 82.4-14.4 63.6-8 114.2 20.2 130.4 6.5 3.8 14.1 5.6 22.5 5.6 27.5 0 63.5-19.6 99.9-53.6 36.4 33.8 72.4 53.2 99.9 53.2 8.4 0 16-1.8 22.6-5.6 28.1-16.2 34.4-66.7 19.9-130.1 62-19.1 102.5-49.9 102.5-82.3zm-130.2-66.7c-3.7 12.9-8.3 26.2-13.5 39.5-4.1-8-8.4-16-13.1-24-4.6-8-9.5-15.8-14.4-23.4 14.2 2.1 27.9 4.7 41 7.9zm-45.8 106.5c-7.8 13.5-15.8 26.3-24.1 38.2-14.9 1.3-30 2-45.2 2-15.1 0-30.2-.7-45-1.9-8.3-11.9-16.4-24.6-24.2-38-7.6-13.1-14.5-26.4-20.8-39.8 6.2-13.4 13.2-26.8 20.7-39.9 7.8-13.5 15.8-26.3 24.1-38.2 14.9-1.3 30-2 45.2-2 15.1 0 30.2.7 45 1.9 8.3 11.9 16.4 24.6 24.2 38 7.6 13.1 14.5 26.4 20.8 39.8-6.3 13.4-13.2 26.8-20.7 39.9zm32.3-13c5.4 13.4 10 26.8 13.8 39.8-13.1 3.2-26.9 5.9-41.2 8 4.9-7.7 9.8-15.6 14.4-23.7 4.6-8 8.9-16.1 13-24.1zM421.2 430c-9.3-9.6-18.6-20.3-27.8-32 9 .4 18.2.7 27.5.7 9.4 0 18.7-.2 27.8-.7-9 11.7-18.3 22.4-27.5 32zm-74.4-58.9c-14.2-2.1-27.9-4.7-41-7.9 3.7-12.9 8.3-26.2 13.5-39.5 4.1 8 8.4 16 13.1 24 4.7 8 9.5 15.8 14.4 23.4zM420.7 163c9.3 9.6 18.6 20.3 27.8 32-9-.4-18.2-.7-27.5-.7-9.4 0-18.7.2-27.8.7 9-11.7 18.3-22.4 27.5-32zm-74 58.9c-4.9 7.7-9.8 15.6-14.4 23.7-4.6 8-8.9 16-13 24-5.4-13.4-10-26.8-13.8-39.8 13.1-3.1 26.9-5.8 41.2-7.9zm-90.5 125.2c-35.4-15.1-58.3-34.9-58.3-50.6 0-15.7 22.9-35.6 58.3-50.6 8.6-3.7 18-7 27.7-10.1 5.7 19.6 13.2 40 22.5 60.9-9.2 20.8-16.6 41.1-22.2 60.6-9.9-3.1-19.3-6.5-28-10.2zM310 490c-13.6-7.8-19.5-37.5-14.9-75.7 1.1-9.4 2.9-19.3 5.1-29.4 19.6 4.8 41 8.5 63.5 10.9 13.5 18.5 27.5 35.3 41.6 50-32.6 30.3-63.2 46.9-84 46.9-4.5-.1-8.3-1-11.3-2.7zm237.2-76.2c4.7 38.2-1.1 67.9-14.6 75.8-3 1.8-6.9 2.6-11.5 2.6-20.7 0-51.4-16.5-84-46.6 14-14.7 28-31.4 41.3-49.9 22.6-2.4 44-6.1 63.6-11 2.3 10.1 4.1 19.8 5.2 29.1zm38.5-66.7c-8.6 3.7-18 7-27.7 10.1-5.7-19.6-13.2-40-22.5-60.9 9.2-20.8 16.6-41.1 22.2-60.6 9.9 3.1 19.3 6.5 28.1 10.2 35.4 15.1 58.3 34.9 58.3 50.6-.1 15.7-23 35.6-58.4 50.6zM320.8 78.4z"/>\n    <circle cx="420.9" cy="296.5" r="45.7"/>\n  </g>\n</svg>\n'
                 }),
-                We = new A({
+                Ye = new M({
                     name: "ui-components:redo",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 0 24 24" width="16">\n  <g class="jp-icon3" fill="#616161">\n      <path d="M0 0h24v24H0z" fill="none"/><path d="M18.4 10.6C16.55 8.99 14.15 8 11.5 8c-4.65 0-8.58 3.03-9.96 7.22L3.9 16c1.05-3.19 4.05-5.5 7.6-5.5 1.95 0 3.73.72 5.12 1.88L13 16h9V7l-3.6 3.6z"/>\n  </g>\n</svg>\n'
                 }),
-                Ye = new A({
+                Xe = new M({
                     name: "ui-components:refresh",
-                    svgstr: v
+                    svgstr: d
                 }),
-                Xe = new A({
+                qe = new M({
                     name: "ui-components:regex",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 20 20">\n  <g class="jp-icon2" fill="#414141">\n    <rect x="2" y="2" width="16" height="16"/>\n  </g>\n\n  <g class="jp-icon-accent2" fill="#FFF">\n    <circle class="st2" cx="5.5" cy="14.5" r="1.5"/>\n    <rect x="12" y="4" class="st2" width="1" height="8"/>\n    <rect x="8.5" y="7.5" transform="matrix(0.866 -0.5 0.5 0.866 -2.3255 7.3219)" class="st2" width="8" height="1"/>\n    <rect x="12" y="4" transform="matrix(0.5 -0.866 0.866 0.5 -0.6779 14.8252)" class="st2" width="1" height="8"/>\n  </g>\n</svg>\n'
                 }),
-                qe = new A({
+                Ze = new M({
                     name: "ui-components:run",
                     svgstr: '<svg height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M8 5v14l11-7z"/>\n    </g>\n</svg>\n'
                 }),
-                Ze = new A({
+                Qe = new M({
                     name: "ui-components:running",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 512 512">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M256 8C119 8 8 119 8 256s111 248 248 248 248-111 248-248S393 8 256 8zm96 328c0 8.8-7.2 16-16 16H176c-8.8 0-16-7.2-16-16V176c0-8.8 7.2-16 16-16h160c8.8 0 16 7.2 16 16v160z"/>\n  </g>\n</svg>\n'
                 }),
-                Qe = new A({
+                $e = new M({
                     name: "ui-components:save",
                     svgstr: '<svg height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M17 3H5c-1.11 0-2 .9-2 2v14c0 1.1.89 2 2 2h14c1.1 0 2-.9 2-2V7l-4-4zm-5 16c-1.66 0-3-1.34-3-3s1.34-3 3-3 3 1.34 3 3-1.34 3-3 3zm3-10H5V5h10v4z"/>\n    </g>\n</svg>\n'
                 }),
-                $e = new A({
+                Je = new M({
                     name: "ui-components:search",
                     svgstr: '<svg viewBox="0 0 18 18" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M12.1,10.9h-0.7l-0.2-0.2c0.8-0.9,1.3-2.2,1.3-3.5c0-3-2.4-5.4-5.4-5.4S1.8,4.2,1.8,7.1s2.4,5.4,5.4,5.4 c1.3,0,2.5-0.5,3.5-1.3l0.2,0.2v0.7l4.1,4.1l1.2-1.2L12.1,10.9z M7.1,10.9c-2.1,0-3.7-1.7-3.7-3.7s1.7-3.7,3.7-3.7s3.7,1.7,3.7,3.7 S9.2,10.9,7.1,10.9z"/>\n  </g>\n</svg>\n'
                 }),
-                Je = new A({
+                et = new M({
                     name: "ui-components:settings",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-icon-selectable" fill="#616161" d="M19.43 12.98c.04-.32.07-.64.07-.98s-.03-.66-.07-.98l2.11-1.65c.19-.15.24-.42.12-.64l-2-3.46c-.12-.22-.39-.3-.61-.22l-2.49 1c-.52-.4-1.08-.73-1.69-.98l-.38-2.65A.488.488 0 0014 2h-4c-.25 0-.46.18-.49.42l-.38 2.65c-.61.25-1.17.59-1.69.98l-2.49-1c-.23-.09-.49 0-.61.22l-2 3.46c-.13.22-.07.49.12.64l2.11 1.65c-.04.32-.07.65-.07.98s.03.66.07.98l-2.11 1.65c-.19.15-.24.42-.12.64l2 3.46c.12.22.39.3.61.22l2.49-1c.52.4 1.08.73 1.69.98l.38 2.65c.03.24.24.42.49.42h4c.25 0 .46-.18.49-.42l.38-2.65c.61-.25 1.17-.59 1.69-.98l2.49 1c.23.09.49 0 .61-.22l2-3.46c.12-.22.07-.49-.12-.64l-2.11-1.65zM12 15.5c-1.93 0-3.5-1.57-3.5-3.5s1.57-3.5 3.5-3.5 3.5 1.57 3.5 3.5-1.57 3.5-3.5 3.5z"/>\n</svg>\n'
                 }),
-                et = new A({
+                tt = new M({
                     name: "ui-components:share",
                     svgstr: '<svg width="16" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M 18 2 C 16.35499 2 15 3.3549904 15 5 C 15 5.1909529 15.021791 5.3771224 15.056641 5.5585938 L 7.921875 9.7207031 C 7.3985399 9.2778539 6.7320771 9 6 9 C 4.3549904 9 3 10.35499 3 12 C 3 13.64501 4.3549904 15 6 15 C 6.7320771 15 7.3985399 14.722146 7.921875 14.279297 L 15.056641 18.439453 C 15.021555 18.621514 15 18.808386 15 19 C 15 20.64501 16.35499 22 18 22 C 19.64501 22 21 20.64501 21 19 C 21 17.35499 19.64501 16 18 16 C 17.26748 16 16.601593 16.279328 16.078125 16.722656 L 8.9433594 12.558594 C 8.9782095 12.377122 9 12.190953 9 12 C 9 11.809047 8.9782095 11.622878 8.9433594 11.441406 L 16.078125 7.2792969 C 16.60146 7.7221461 17.267923 8 18 8 C 19.64501 8 21 6.6450096 21 5 C 21 3.3549904 19.64501 2 18 2 z M 18 4 C 18.564129 4 19 4.4358706 19 5 C 19 5.5641294 18.564129 6 18 6 C 17.435871 6 17 5.5641294 17 5 C 17 4.4358706 17.435871 4 18 4 z M 6 11 C 6.5641294 11 7 11.435871 7 12 C 7 12.564129 6.5641294 13 6 13 C 5.4358706 13 5 12.564129 5 12 C 5 11.435871 5.4358706 11 6 11 z M 18 18 C 18.564129 18 19 18.435871 19 19 C 19 19.564129 18.564129 20 18 20 C 17.435871 20 17 19.564129 17 19 C 17 18.435871 17.435871 18 18 18 z"/>\n  </g>\n</svg>\n'
                 }),
-                tt = new A({
+                nt = new M({
                     name: "ui-components:spreadsheet",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <path class="jp-icon-contrast1 jp-icon-selectable" fill="#4CAF50" d="M2.2 2.2v17.6h17.6V2.2H2.2zm15.4 7.7h-5.5V4.4h5.5v5.5zM9.9 4.4v5.5H4.4V4.4h5.5zm-5.5 7.7h5.5v5.5H4.4v-5.5zm7.7 5.5v-5.5h5.5v5.5h-5.5z"/>\n</svg>\n'
                 }),
-                nt = new A({
+                ct = new M({
                     name: "ui-components:stop",
                     svgstr: '<svg height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M0 0h24v24H0z" fill="none"/>\n        <path d="M6 6h12v12H6z"/>\n    </g>\n</svg>\n'
                 }),
-                ct = new A({
+                ot = new M({
                     name: "ui-components:tab",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M21 3H3c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h18c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zm0 16H3V5h10v4h8v10z"/>\n  </g>\n</svg>\n'
                 }),
-                ot = new A({
+                at = new M({
                     name: "ui-components:table-rows",
                     svgstr: '<svg height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M0 0h24v24H0z" fill="none"/>\n        <path d="M21,8H3V4h18V8z M21,10H3v4h18V10z M21,16H3v4h18V16z"/>\n    </g>\n</svg>'
                 }),
-                at = new A({
+                rt = new M({
                     name: "ui-components:tag",
                     svgstr: '<svg width="28" height="28" viewBox="0 0 43 28" xmlns="http://www.w3.org/2000/svg">\n\t<g class="jp-icon3" fill="#616161">\n\t\t<path d="M28.8332 12.334L32.9998 16.5007L37.1665 12.334H28.8332Z"/>\n\t\t<path d="M16.2095 21.6104C15.6873 22.1299 14.8443 22.1299 14.3248 21.6104L6.9829 14.7245C6.5724 14.3394 6.08313 13.6098 6.04786 13.0482C5.95347 11.5288 6.02002 8.61944 6.06621 7.07695C6.08281 6.51477 6.55548 6.04347 7.11804 6.03055C9.08863 5.98473 13.2638 5.93579 13.6518 6.32425L21.7369 13.639C22.256 14.1585 21.7851 15.4724 21.262 15.9946L16.2095 21.6104ZM9.77585 8.265C9.33551 7.82566 8.62351 7.82566 8.1828 8.265C7.74346 8.70571 7.74346 9.41733 8.1828 9.85667C8.62382 10.2964 9.33582 10.2964 9.77585 9.85667C10.2156 9.41733 10.2156 8.70533 9.77585 8.265Z"/>\n\t</g>\n</svg>\n'
                 }),
-                rt = new A({
+                st = new M({
                     name: "ui-components:terminal",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24" >\n    <rect class="jp-terminal-icon-background-color jp-icon-selectable" width="20" height="20" transform="translate(2 2)" fill="#333333"/>\n    <path class="jp-terminal-icon-color jp-icon-selectable-inverse" d="M5.05664 8.76172C5.05664 8.59766 5.03125 8.45312 4.98047 8.32812C4.93359 8.19922 4.85547 8.08203 4.74609 7.97656C4.64062 7.87109 4.5 7.77539 4.32422 7.68945C4.15234 7.59961 3.94336 7.51172 3.69727 7.42578C3.30273 7.28516 2.94336 7.13672 2.61914 6.98047C2.29492 6.82422 2.01758 6.64258 1.78711 6.43555C1.56055 6.22852 1.38477 5.98828 1.25977 5.71484C1.13477 5.4375 1.07227 5.10938 1.07227 4.73047C1.07227 4.39844 1.12891 4.0957 1.24219 3.82227C1.35547 3.54492 1.51562 3.30469 1.72266 3.10156C1.92969 2.89844 2.17969 2.73437 2.47266 2.60938C2.76562 2.48438 3.0918 2.4043 3.45117 2.36914V1.10938H4.38867V2.38086C4.74023 2.42773 5.05664 2.52344 5.33789 2.66797C5.61914 2.8125 5.85742 3.00195 6.05273 3.23633C6.25195 3.4668 6.4043 3.74023 6.50977 4.05664C6.61914 4.36914 6.67383 4.7207 6.67383 5.11133H5.04492C5.04492 4.63867 4.9375 4.28125 4.72266 4.03906C4.50781 3.79297 4.2168 3.66992 3.84961 3.66992C3.65039 3.66992 3.47656 3.69727 3.32812 3.75195C3.18359 3.80273 3.06445 3.87695 2.9707 3.97461C2.87695 4.06836 2.80664 4.17969 2.75977 4.30859C2.7168 4.4375 2.69531 4.57812 2.69531 4.73047C2.69531 4.88281 2.7168 5.01953 2.75977 5.14062C2.80664 5.25781 2.88281 5.36719 2.98828 5.46875C3.09766 5.57031 3.24023 5.66797 3.41602 5.76172C3.5918 5.85156 3.81055 5.94336 4.07227 6.03711C4.4668 6.18555 4.82422 6.33984 5.14453 6.5C5.46484 6.65625 5.73828 6.83984 5.96484 7.05078C6.19531 7.25781 6.37109 7.5 6.49219 7.77734C6.61719 8.05078 6.67969 8.375 6.67969 8.75C6.67969 9.09375 6.62305 9.4043 6.50977 9.68164C6.39648 9.95508 6.23438 10.1914 6.02344 10.3906C5.8125 10.5898 5.55859 10.75 5.26172 10.8711C4.96484 10.9883 4.63281 11.0645 4.26562 11.0996V12.248H3.33398V11.0996C3.00195 11.0684 2.67969 10.9961 2.36719 10.8828C2.05469 10.7656 1.77734 10.5977 1.53516 10.3789C1.29688 10.1602 1.10547 9.88477 0.960938 9.55273C0.816406 9.2168 0.744141 8.81445 0.744141 8.3457H2.37891C2.37891 8.62695 2.41992 8.86328 2.50195 9.05469C2.58398 9.24219 2.68945 9.39258 2.81836 9.50586C2.95117 9.61523 3.10156 9.69336 3.26953 9.74023C3.4375 9.78711 3.60938 9.81055 3.78516 9.81055C4.20312 9.81055 4.51953 9.71289 4.73438 9.51758C4.94922 9.32227 5.05664 9.07031 5.05664 8.76172ZM13.418 12.2715H8.07422V11H13.418V12.2715Z" transform="translate(3.95264 6)" fill="white"/>\n</svg>\n'
                 }),
-                st = new A({
+                lt = new M({
                     name: "ui-components:text-editor",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <path class="jp-text-editor-icon-color jp-icon-selectable" fill="#616161" d="M15 15H3v2h12v-2zm0-8H3v2h12V7zM3 13h18v-2H3v2zm0 8h18v-2H3v2zM3 3v2h18V3H3z"/>\n</svg>\n'
                 }),
-                lt = new A({
+                it = new M({
                     name: "ui-components:toc",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">\n  <g class="jp-icon3 jp-icon-selectable" fill="#616161">\n    <path d="M7,5H21V7H7V5M7,13V11H21V13H7M4,4.5A1.5,1.5 0 0,1 5.5,6A1.5,1.5 0 0,1 4,7.5A1.5,1.5 0 0,1 2.5,6A1.5,1.5 0 0,1 4,4.5M4,10.5A1.5,1.5 0 0,1 5.5,12A1.5,1.5 0 0,1 4,13.5A1.5,1.5 0 0,1 2.5,12A1.5,1.5 0 0,1 4,10.5M7,19V17H21V19H7M4,16.5A1.5,1.5 0 0,1 5.5,18A1.5,1.5 0 0,1 4,19.5A1.5,1.5 0 0,1 2.5,18A1.5,1.5 0 0,1 4,16.5Z" />\n  </g>\n</svg>\n'
                 }),
-                it = new A({
+                ht = new M({
                     name: "ui-components:tree-view",
                     svgstr: '<svg height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">\n    <g class="jp-icon3" fill="#616161">\n        <path d="M0 0h24v24H0z" fill="none"/>\n        <path d="M22 11V3h-7v3H9V3H2v8h7V8h2v10h4v3h7v-8h-7v3h-2V8h2v3z"/>\n    </g>\n</svg>'
                 }),
-                ht = new A({
+                pt = new M({
                     name: "ui-components:trusted",
                     svgstr: '<svg fill="none" xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 25">\n    <path class="jp-icon2" stroke="#333333" stroke-width="2" transform="translate(2 3)" d="M1.86094 11.4409C0.826448 8.77027 0.863779 6.05764 1.24907 4.19932C2.48206 3.93347 4.08068 3.40347 5.60102 2.8449C7.23549 2.2444 8.85666 1.5815 9.9876 1.09539C11.0597 1.58341 12.6094 2.2444 14.218 2.84339C15.7503 3.41394 17.3995 3.95258 18.7539 4.21385C19.1364 6.07177 19.1709 8.77722 18.139 11.4409C17.0303 14.3032 14.6668 17.1844 9.99999 18.9354C5.3332 17.1844 2.96968 14.3032 1.86094 11.4409Z"/>\n    <path class="jp-icon2" fill="#333333" stroke="#333333" transform="translate(8 9.86719)" d="M2.86015 4.86535L0.726549 2.99959L0 3.63045L2.86015 6.13157L8 0.630872L7.27857 0L2.86015 4.86535Z"/>\n</svg>\n'
                 }),
-                pt = new A({
+                ut = new M({
                     name: "ui-components:undo",
                     svgstr: '<svg viewBox="0 0 24 24" width="16" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M12.5 8c-2.65 0-5.05.99-6.9 2.6L2 7v9h9l-3.62-3.62c1.39-1.16 3.16-1.88 5.12-1.88 3.54 0 6.55 2.31 7.6 5.5l2.37-.78C21.08 11.03 17.15 8 12.5 8z"/>\n  </g>\n</svg>\n'
                 }),
-                ut = new A({
+                vt = new M({
                     name: "ui-components:user",
                     svgstr: '<svg width="16" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>\n  </g>\n</svg>'
                 }),
-                vt = new A({
+                dt = new M({
                     name: "ui-components:users",
                     svgstr: '<svg width="24" height="24" version="1.1" viewBox="0 0 36 24" xmlns="http://www.w3.org/2000/svg">\n <g class="jp-icon3" transform="matrix(1.7327 0 0 1.7327 -3.6282 .099577)" fill="#616161">\n  <path transform="matrix(1.5,0,0,1.5,0,-6)" d="m12.186 7.5098c-1.0535 0-1.9757 0.5665-2.4785 1.4102 0.75061 0.31277 1.3974 0.82648 1.873 1.4727h3.4863c0-1.592-1.2889-2.8828-2.8809-2.8828z"/>\n  <path d="m20.465 2.3895a2.1885 2.1885 0 0 1-2.1884 2.1885 2.1885 2.1885 0 0 1-2.1885-2.1885 2.1885 2.1885 0 0 1 2.1885-2.1885 2.1885 2.1885 0 0 1 2.1884 2.1885z"/>\n  <path transform="matrix(1.5,0,0,1.5,0,-6)" d="m3.5898 8.4219c-1.1126 0-2.0137 0.90111-2.0137 2.0137h2.8145c0.26797-0.37309 0.5907-0.70435 0.95898-0.97852-0.34433-0.61688-1.0031-1.0352-1.7598-1.0352z"/>\n  <path d="m6.9154 4.623a1.5294 1.5294 0 0 1-1.5294 1.5294 1.5294 1.5294 0 0 1-1.5294-1.5294 1.5294 1.5294 0 0 1 1.5294-1.5294 1.5294 1.5294 0 0 1 1.5294 1.5294z"/>\n  <path d="m6.135 13.535c0-3.2392 2.6259-5.865 5.865-5.865 3.2392 0 5.865 2.6259 5.865 5.865z"/>\n  <circle cx="12" cy="3.7685" r="2.9685"/>\n </g>\n</svg>\n'
                 }),
-                dt = new A({
+                mt = new M({
                     name: "ui-components:vega",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <g class="jp-icon1 jp-icon-selectable" fill="#212121">\n    <path d="M10.6 5.4l2.2-3.2H2.2v7.3l4-6.6z"/>\n    <path d="M15.8 2.2l-4.4 6.6L7 6.3l-4.8 8v5.5h17.6V2.2h-4zm-7 15.4H5.5v-4.4h3.3v4.4zm4.4 0H9.8V9.8h3.4v7.8zm4.4 0h-3.4V6.5h3.4v11.1z"/>\n  </g>\n</svg>\n'
                 }),
-                mt = new A({
+                ft = new M({
                     name: "ui-components:yaml",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22">\n  <g class="jp-icon-contrast2 jp-icon-selectable" fill="#D81B60">\n    <path d="M7.2 18.6v-5.4L3 5.6h3.3l1.4 3.1c.3.9.6 1.6 1 2.5.3-.8.6-1.6 1-2.5l1.4-3.1h3.4l-4.4 7.6v5.5l-2.9-.1z"/>\n    <circle class="st0" cx="17.6" cy="16.5" r="2.1"/>\n    <circle class="st0" cx="17.6" cy="11" r="2.1"/>\n  </g>\n</svg>\n'
                 }),
-                ft = "jp-DefaultStyle";
-            const Et = "jp-HTMLSelect";
-            class zt extends l.Component {
+                Et = "jp-DefaultStyle";
+            const zt = "jp-HTMLSelect";
+            class gt extends l.Component {
                 render() {
                     const e = this.props,
                         {
                             className: t,
                             defaultStyle: n = !0,
                             disabled: c,
                             elementRef: o,
                             iconProps: a,
-                            icon: r = B,
+                            icon: r = k,
                             options: s = []
                         } = e,
                         i = function(e, t) {
                             var n = {};
                             for (var c in e) Object.prototype.hasOwnProperty.call(e, c) && t.indexOf(c) < 0 && (n[c] = e[c]);
                             if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                                 var o = 0;
                                 for (c = Object.getOwnPropertySymbols(e); o < c.length; o++) t.indexOf(c[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, c[o]) && (n[c[o]] = e[c[o]])
                             }
                             return n
                         }(e, ["className", "defaultStyle", "disabled", "elementRef", "iconProps", "icon", "options"]),
-                        h = z(Et, {
-                            [ft]: n
+                        h = g(zt, {
+                            [Et]: n
                         }, t),
                         p = s.map((e => {
                             const t = "object" == typeof e ? e : {
                                 value: e
                             };
                             return l.createElement("option", Object.assign({}, t, {
                                 key: t.value
@@ -15120,34 +15121,34 @@
                         tag: "span",
                         stylesheet: "select",
                         right: "7px",
                         top: "5px"
                     }, a))))
                 }
             }
-            var gt, _t = n(23203),
-                Lt = n(36e3),
-                Ct = n(42051);
+            var _t, Lt = n(23203),
+                Ct = n(36e3),
+                At = n(42051);
             ! function(e) {
                 e.DEFAULT_RANK = 100
-            }(gt || (gt = {}));
-            class At extends Ct.Menu {
+            }(_t || (_t = {}));
+            class Mt extends At.Menu {
                 constructor(e) {
                     var t;
                     super(e), this._ranks = [], this._rank = e.rank, this._includeSeparators = null === (t = e.includeSeparators) || void 0 === t || t
                 }
                 get menu() {
                     return this
                 }
                 get rank() {
                     return this._rank
                 }
                 addGroup(e, t) {
-                    if (0 === e.length) return new Lt.DisposableDelegate((() => {}));
-                    const n = null != t ? t : gt.DEFAULT_RANK,
+                    if (0 === e.length) return new Ct.DisposableDelegate((() => {}));
+                    const n = null != t ? t : _t.DEFAULT_RANK,
                         c = e.map((e => {
                             var t;
                             return Object.assign(Object.assign({}, e), {
                                 rank: null !== (t = e.rank) && void 0 !== t ? t : n
                             })
                         })).sort(((e, t) => e.rank - t.rank));
                     let o = this._ranks.findIndex((e => c[0].rank < e));
@@ -15155,15 +15156,15 @@
                     const a = [];
                     return this._includeSeparators && a.push(this.insertItem(o++, {
                         type: "separator",
                         rank: n
                     })), a.push(...c.map((e => this.insertItem(o++, e)))), this._includeSeparators && a.push(this.insertItem(o++, {
                         type: "separator",
                         rank: n
-                    })), new Lt.DisposableDelegate((() => {
+                    })), new Ct.DisposableDelegate((() => {
                         a.forEach((e => e.dispose()))
                     }))
                 }
                 addItem(e) {
                     let t = -1;
                     return e.rank && (t = this._ranks.findIndex((t => e.rank < t))), t < 0 && (t = this._ranks.length), this.insertItem(t, e)
                 }
@@ -15175,23 +15176,23 @@
                 }
                 getRankAt(e) {
                     return this._ranks[e]
                 }
                 insertItem(e, t) {
                     var n, c;
                     const o = Math.max(0, Math.min(e, this._ranks.length));
-                    _t.ArrayExt.insert(this._ranks, o, null !== (n = t.rank) && void 0 !== n ? n : Math.max(gt.DEFAULT_RANK, null !== (c = this._ranks[this._ranks.length - 1]) && void 0 !== c ? c : gt.DEFAULT_RANK));
+                    Lt.ArrayExt.insert(this._ranks, o, null !== (n = t.rank) && void 0 !== n ? n : Math.max(_t.DEFAULT_RANK, null !== (c = this._ranks[this._ranks.length - 1]) && void 0 !== c ? c : _t.DEFAULT_RANK));
                     const a = super.insertItem(o, t);
-                    return new Mt(a, this)
+                    return new Tt(a, this)
                 }
                 removeItemAt(e) {
-                    _t.ArrayExt.removeAt(this._ranks, e), super.removeItemAt(e)
+                    Lt.ArrayExt.removeAt(this._ranks, e), super.removeItemAt(e)
                 }
             }
-            class Mt {
+            class Tt {
                 constructor(e, t) {
                     this._item = new WeakRef(e), this._menu = t;
                     const n = e => {
                         e.disposed.disconnect(n, this), this.dispose()
                     };
                     this._menu.disposed.connect(n, this)
                 }
@@ -15249,15 +15250,15 @@
                 dispose() {
                     if (this._isDisposed) return;
                     this._isDisposed = !0;
                     const e = this._item.deref();
                     e && !this._menu.isDisposed && this._menu.removeItem(e), p.Signal.clearData(this)
                 }
             }
-            class Tt extends Ct.Widget {
+            class yt extends At.Widget {
                 constructor() {
                     super(), this._button = document.createElement("button"), this._label = document.createElement("label"), this._valueChanged = new p.Signal(this), this._button.className = "jp-switch", this._button.setAttribute("role", "switch"), this._label.className = "jp-switch-label";
                     const e = document.createElement("div");
                     e.className = "jp-switch-track", e.setAttribute("aria-hidden", "true"), this._button.appendChild(this._label), this._button.appendChild(e), this.node.appendChild(this._button)
                 }
                 get value() {
                     return this._value
@@ -15292,53 +15293,53 @@
                 onAfterAttach() {
                     this._button.addEventListener("click", this)
                 }
                 onBeforeDetach() {
                     this._button.removeEventListener("click", this)
                 }
             }
-            var yt = n(32886);
-            const Ot = ue.bindprops({
+            var Ot = n(32886);
+            const Ht = ve.bindprops({
                 stylesheet: "commandPaletteHeader",
                 className: "jp-icon-hoverShow-content"
             });
-            var Ht;
+            var Rt;
             ! function(e) {
-                class t extends Ct.CommandPalette.Renderer {
+                class t extends At.CommandPalette.Renderer {
                     renderHeader(e) {
                         const t = this.formatHeader(e);
-                        return yt.h.li({
-                            className: z("lm-CommandPalette-header", "jp-icon-hoverShow", "p-CommandPalette-header")
-                        }, t, yt.h.span(Ot))
+                        return Ot.h.li({
+                            className: g("lm-CommandPalette-header", "jp-icon-hoverShow", "p-CommandPalette-header")
+                        }, t, Ot.h.span(Ht))
                     }
                     renderItemIcon(e) {
                         const t = this.createIconClass(e);
-                        return e.item.isToggled ? yt.h.div({
+                        return e.item.isToggled ? Ot.h.div({
                             className: t
-                        }, Y, e.item.iconLabel) : "string" == typeof e.item.icon ? yt.h.div({
+                        }, X, e.item.iconLabel) : "string" == typeof e.item.icon ? Ot.h.div({
                             className: t
-                        }, e.item.iconLabel) : yt.h.div({
+                        }, e.item.iconLabel) : Ot.h.div({
                             className: t
                         }, e.item.icon, e.item.iconLabel)
                     }
                     createIconClass(e) {
                         let t = "lm-CommandPalette-itemIcon";
-                        return t += " p-CommandPalette-itemIcon", z(d.styleClass({
+                        return t += " p-CommandPalette-itemIcon", g(m.styleClass({
                             stylesheet: "commandPaletteItem"
                         }), e.item.iconClass, "lm-CommandPalette-itemIcon p-CommandPalette-itemIcon")
                     }
                 }
                 e.Renderer = t, e.defaultRenderer = new t
-            }(Ht || (Ht = {}));
-            const Rt = G.bindprops({
+            }(Rt || (Rt = {}));
+            const Nt = j.bindprops({
                 stylesheet: "menuItem"
             });
-            class Nt extends Ct.ContextMenu {
+            class It extends At.ContextMenu {
                 constructor(e) {
-                    super(e), this._isDisposed = !1, this._opened = new p.Signal(this), this.menu = new It(e)
+                    super(e), this._isDisposed = !1, this._opened = new p.Signal(this), this.menu = new Vt(e)
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get opened() {
                     return this._opened
                 }
@@ -15347,115 +15348,115 @@
                 }
                 open(e) {
                     if (this._isDisposed) return !1;
                     const t = super.open(e);
                     return t && this._opened.emit(), t
                 }
             }
-            class It extends Ct.Menu {
+            class Vt extends At.Menu {
                 constructor(e) {
-                    e.renderer = e.renderer || It.defaultRenderer, super(e)
+                    e.renderer = e.renderer || Vt.defaultRenderer, super(e)
                 }
                 insertItem(e, t) {
-                    return t.submenu && It.overrideDefaultRenderer(t.submenu), super.insertItem(e, t)
+                    return t.submenu && Vt.overrideDefaultRenderer(t.submenu), super.insertItem(e, t)
                 }
             }! function(e) {
                 e.overrideDefaultRenderer = function t(n) {
-                    n.renderer === Ct.Menu.defaultRenderer && (n.renderer = e.defaultRenderer);
+                    n.renderer === At.Menu.defaultRenderer && (n.renderer = e.defaultRenderer);
                     const c = n.insertItem.bind(n);
                     n.insertItem = (t, n) => (n.submenu && e.overrideDefaultRenderer(n.submenu), c(t, n));
                     for (const e of n._items) e.submenu && t(e.submenu)
                 };
-                class t extends Ct.Menu.Renderer {
+                class t extends At.Menu.Renderer {
                     renderIcon(e) {
                         const t = this.createIconClass(e);
-                        return e.item.isToggled ? yt.h.div({
+                        return e.item.isToggled ? Ot.h.div({
                             className: t
-                        }, Y, e.item.iconLabel) : "string" == typeof e.item.icon ? yt.h.div({
-                            className: z(t, "jp-Icon")
-                        }, e.item.iconLabel) : yt.h.div({
+                        }, X, e.item.iconLabel) : "string" == typeof e.item.icon ? Ot.h.div({
+                            className: g(t, "jp-Icon")
+                        }, e.item.iconLabel) : Ot.h.div({
                             className: t
                         }, e.item.icon, e.item.iconLabel)
                     }
                     createIconClass(e) {
                         let t = "lm-Menu-itemIcon";
-                        return t += " p-Menu-itemIcon", "separator" === e.item.type ? z(e.item.iconClass, t) : z(d.styleClass({
+                        return t += " p-Menu-itemIcon", "separator" === e.item.type ? g(e.item.iconClass, t) : g(m.styleClass({
                             stylesheet: "menuItem"
                         }), e.item.iconClass, t)
                     }
                     renderSubmenu(e) {
                         const t = "lm-Menu-itemSubmenuIcon p-Menu-itemSubmenuIcon";
-                        return "submenu" === e.item.type ? yt.h.div({
+                        return "submenu" === e.item.type ? Ot.h.div({
                             className: t
-                        }, Rt) : yt.h.div({
+                        }, Nt) : Ot.h.div({
                             className: t
                         })
                     }
                 }
                 e.Renderer = t, e.defaultRenderer = new t
-            }(It || (It = {}));
-            var Vt = n(56956);
-            class St extends Ct.TabBar {
+            }(Vt || (Vt = {}));
+            var St = n(56956);
+            class bt extends At.TabBar {
                 constructor(e = {}) {
-                    e.renderer = e.renderer || St.defaultRenderer, super(e);
-                    const t = (e && e.translator || Vt.nullTranslator).load("jupyterlab");
-                    b.element({
+                    e.renderer = e.renderer || bt.defaultRenderer, super(e);
+                    const t = (e && e.translator || St.nullTranslator).load("jupyterlab");
+                    w.element({
                         container: this.addButtonNode,
                         title: t.__("New Launcher")
                     })
                 }
             }! function(e) {
-                class t extends Ct.TabBar.Renderer {
+                class t extends At.TabBar.Renderer {
                     renderCloseIcon(e) {
-                        const t = z("jp-icon-hover lm-TabBar-tabCloseIcon", d.styleClass({
+                        const t = g("jp-icon-hover lm-TabBar-tabCloseIcon", m.styleClass({
                             elementPosition: "center",
                             height: "16px",
                             width: "16px"
                         }));
-                        return (0, yt.hpass)("div", {
+                        return (0, Ot.hpass)("div", {
                             className: t
-                        }, Q)
+                        }, $)
                     }
                 }
                 e.Renderer = t, e.defaultRenderer = new t
-            }(St || (St = {}));
-            class bt extends Ct.DockPanel {
+            }(bt || (bt = {}));
+            class wt extends At.DockPanel {
                 constructor(e = {}) {
-                    e.renderer = e.renderer || bt.defaultRenderer, super(e)
+                    e.renderer = e.renderer || wt.defaultRenderer, super(e)
                 }
             }! function(e) {
-                class t extends Ct.DockPanel.Renderer {
+                class t extends At.DockPanel.Renderer {
                     createTabBar() {
-                        const e = new St;
+                        const e = new bt;
                         return e.addClass("lm-DockPanel-tabBar"), e
                     }
                 }
                 e.Renderer = t, e.defaultRenderer = new t
-            }(bt || (bt = {}));
-            class wt extends Ct.TabPanel {
+            }(wt || (wt = {}));
+            class Pt extends At.TabPanel {
                 constructor(e = {}) {
-                    e.renderer = e.renderer || St.defaultRenderer, super(e)
+                    e.renderer = e.renderer || bt.defaultRenderer, super(e)
                 }
             }
-            const Pt = new h.Token("@jupyterlab/ui-components:ILabIconManager");
-            class Dt {
+            const Dt = new h.Token("@jupyterlab/ui-components:ILabIconManager");
+            class xt {
                 constructor() {
                     this._renderers = {}
                 }
                 addRenderer(e, t) {
                     return !this._renderers[e] && (this._renderers[e] = t, !0)
                 }
                 get renderers() {
                     return this._renderers
                 }
                 getRenderer(e) {
                     return this._renderers[e]
                 }
             }
-            const xt = new h.Token("@jupyterlab/ui-components:ISettingEditorRegistry")
+            const Bt = new h.Token("@jupyterlab/ui-components:ISettingEditorRegistry")
         },
         62680: (e, t, n) => {
             "use strict";
             var c = n(67286),
                 o = n(89429),
                 a = o(c("String.prototype.indexOf"));
             e.exports = function(e, t) {
@@ -16845,15 +16846,15 @@
             var u = p;
             t.default = u, e.exports = t.default
         },
         34674: (e, t, n) => {
             "use strict";
             t.__esModule = !0, t.default = void 0, r(n(13980));
             var c = r(n(97505)),
-                o = n(28316),
+                o = n(24627),
                 a = r(n(80996));
 
             function r(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             }
@@ -16929,15 +16930,15 @@
                         for (var n in e)
                             if (Object.prototype.hasOwnProperty.call(e, n)) {
                                 var c = Object.defineProperty && Object.getOwnPropertyDescriptor ? Object.getOwnPropertyDescriptor(e, n) : {};
                                 c.get || c.set ? Object.defineProperty(t, n, c) : t[n] = e[n]
                             } return t.default = e, t
                 }(n(13980)),
                 o = s(n(97505)),
-                a = s(n(28316)),
+                a = s(n(24627)),
                 r = n(46847);
 
             function s(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             }
```

### Comparing `voici-0.4.0/voici/static/build/4963.js.LICENSE.txt` & `voici-0.4.1/voici/static/build/4963.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/4977.js` & `voici-0.4.1/voici/static/build/4977.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/5188.js` & `voici-0.4.1/voici/static/build/5188.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/5291.js` & `voici-0.4.1/voici/static/build/5291.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/53.js` & `voici-0.4.1/voici/static/build/53.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/5403.js` & `voici-0.4.1/voici/static/build/5403.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/5445.js` & `voici-0.4.1/voici/static/build/5445.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/5474.js` & `voici-0.4.1/voici/static/build/5474.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5474], {
         27693: e => {
             e.exports = {
                 name: "@voila-dashboards/voici",
-                version: "0.4.0",
+                version: "0.4.1",
                 description: "The Voici Frontend",
                 author: "Voilà contributors",
                 license: "BSD-3-Clause",
                 main: "lib/index.js",
                 browserslist: ">0.8%, not ie 11, not op_mini all, not dead",
                 dependencies: {
                     "@jupyter-widgets/base": "^6.0.1",
@@ -49,15 +49,16 @@
                     "@lumino/dragdrop": "^1.10.2",
                     "@lumino/messaging": "^1.7.2",
                     "@lumino/properties": "^1.5.2",
                     "@lumino/signaling": "^1.7.2",
                     "@lumino/virtualdom": "^1.11.2",
                     "@lumino/widgets": "^1.26.2",
                     "@voila-dashboards/voila": "^0.5.0-alpha.3",
-                    react: "^17.0.1"
+                    react: "^17.0.1",
+                    "react-dom": "^17.0.1"
                 },
                 devDependencies: {
                     "@babel/core": "^7.2.2",
                     "@babel/preset-env": "^7.3.1",
                     "@jupyterlab/builder": "^3.0.0",
                     "@types/node": "^18.8.3",
                     "babel-loader": "^8.0.5",
@@ -94,23 +95,23 @@
                 publishConfig: {
                     access: "public"
                 }
             }
         },
         65474: (e, t, n) => {
             "use strict";
-            n.r(t), n(71024);
+            n.r(t), n(71024), n(24627);
             var i = n(59110),
                 a = n(94456),
                 r = n(7631),
                 o = n(22312),
                 s = n(75238),
                 l = n(73198),
-                c = n(40049),
-                u = n(12299),
+                u = n(40049),
+                c = n(12299),
                 d = n(35918),
                 p = n(92233),
                 g = n(42051);
             const m = n(27693),
                 h = "application/vnd.jupyter.widget-view+json";
             class f extends s.JupyterFrontEnd {
                 constructor(e) {
@@ -170,15 +171,15 @@
                 async renderWidgets() {
                     var e, t, n;
                     const a = this._serviceManager;
                     if (!a) return void console.error("Missing service manager");
                     await a.ready;
                     const r = a.sessions;
                     await r.ready;
-                    const o = new c.NotebookModel;
+                    const o = new u.NotebookModel;
                     o.fromString(i.PageConfig.getOption("notebookSrc"));
                     let s = o.metadata.get("kernelspec");
                     s || (s = {
                         name: "python"
                     });
                     const l = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
                     let p;
@@ -196,79 +197,68 @@
                             type: "notebook",
                             kernel: p
                         }),
                         m = g.kernel;
                     m ? m.connectionStatusChanged.connect((async (e, t) => {
                         if ("connected" === t) {
                             window.update_loading_text(0, 0, "Starting up kernel...");
-                            const e = new u.RenderMimeRegistry({
-                                    initialFactories: u.standardRendererFactories
+                            const e = new c.RenderMimeRegistry({
+                                    initialFactories: c.standardRendererFactories
                                 }),
                                 t = new d.KernelWidgetManager(m, e);
                             if (e.removeMimeType(h), e.addFactory({
                                     safe: !1,
                                     mimeTypes: [h],
                                     createRenderer: e => new d.WidgetRenderer(e, t)
                                 }, -10), this._widgetManagerPromise.resolve(t), !g.kernel) return;
                             await new Promise((e => setTimeout(e, 500)));
                             let n = !1;
-                            const a = i.PageConfig.getOption("packagesSrc");
                             m.statusChanged.connect((async (t, i) => {
                                 n || "idle" !== i || (n = !0, await b.executeCells({
-                                    packages: a,
                                     source: o,
                                     rendermime: e,
                                     kernel: g.kernel
                                 }))
                             }))
                         }
                     })) : console.error("Can not start kernel")
                 }
             }
             var b;
             ! function(e) {
                 e.executeCells = async function(e) {
                     var t, n;
                     const {
-                        packages: i,
-                        source: a,
-                        rendermime: r,
-                        kernel: o
-                    } = e;
-                    if (i && i.length > 0) {
-                        window.update_loading_text(0, 0, "Installing dependencies");
-                        const e = o.requestExecute({
-                            code: i
-                        });
-                        await e.done
-                    }
-                    const s = a.cells.length;
-                    for (let e = 0; e < s; e++) {
-                        const i = a.cells.get(e);
-                        if (window.update_loading_text(e + 1, s, null), "code" !== i.type) {
-                            e === s - 1 && window.display_cells();
+                        source: i,
+                        rendermime: a,
+                        kernel: r
+                    } = e, o = i.cells.length;
+                    for (let e = 0; e < o; e++) {
+                        const s = i.cells.get(e);
+                        if (window.update_loading_text(e + 1, o, null), "code" !== s.type) {
+                            e === o - 1 && window.display_cells();
                             continue
                         }
-                        const c = new l.OutputAreaModel({
+                        const u = new l.OutputAreaModel({
                                 trusted: !0
                             }),
-                            u = new l.SimplifiedOutputArea({
-                                model: c,
-                                rendermime: r
+                            c = new l.SimplifiedOutputArea({
+                                model: u,
+                                rendermime: a
                             });
-                        u.future = o.requestExecute({
-                            code: i.value.text
-                        }), await u.future.done;
+                        c.future = r.requestExecute({
+                            code: s.value.text
+                        }), await c.future.done;
                         const d = document.querySelector(`[cell-index="${e+1}"]`);
-                        if (d && u.node.childNodes.length > 0) {
+                        if (d && c.node.childNodes.length > 0) {
                             null === (t = d.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
                             const e = document.createElement("div");
-                            e.classList.add("jp-Cell-outputWrapper"), null === (n = d.lastElementChild) || void 0 === n || n.appendChild(e), u.node.classList.add("jp-Cell-outputArea", "jp-OutputArea-child"), g.Widget.attach(u, e)
+                            e.classList.add("jp-Cell-outputWrapper"), null === (n = d.lastElementChild) || void 0 === n || n.appendChild(e), c.node.classList.add("jp-Cell-outputArea", "jp-OutputArea-child"), g.Widget.attach(c, e)
                         }
-                        e === s - 1 && (window.display_cells(), window.dispatchEvent(new Event("resize")))
+                        e === o - 1 && (window.display_cells(), window.dispatchEvent(new Event("resize")))
                     }
                 }
             }(b || (b = {}));
             var w = n(67651),
                 y = n(37782);
             const v = {
                     id: "@voila-dashboards/voici:widget-manager",
@@ -280,53 +270,53 @@
                         return {
                             registerWidget: async e => {
                                 (await t.promise).register(e)
                             }
                         }
                     }
                 },
-                P = {
+                j = {
                     id: "@voila-dashboards/voici:theme-manager",
                     autoStart: !0,
                     optional: [y.IThemeManager],
                     activate: (e, t) => {
                         if (!t) return;
                         const n = window.location.search,
                             a = new URLSearchParams(n).get("theme"),
                             r = i.PageConfig.getOption("jpThemeName");
                         let o = a ? decodeURIComponent(a) : r;
                         o = o || "light", "dark" !== o && "JupyterLab Dark" !== o || (o = "JupyterLab Dark"), "light" !== o && "JupyterLab Light" !== o || (o = "JupyterLab Light"), t.themeChanged.connect((() => {
                             t.theme !== o && t.setTheme(o)
                         }))
                     }
                 },
-                j = [o.pathsPlugin, o.translatorPlugin, v, P];
+                P = [o.pathsPlugin, o.translatorPlugin, v, j];
             async function k(e, t) {
                 try {
                     return (await window._JUPYTERLAB[e].get(t))()
                 } catch (n) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${t}`), n
                 }
             }
 
             function* C(e, t) {
                 let n;
                 n = Object.prototype.hasOwnProperty.call(e, "__esModule") ? e.default : e;
                 const a = Array.isArray(n) ? n : [n];
                 for (const e of a) i.PageConfig.Extension.isDisabled(e.id) || t.includes(e.id) || t.includes(e.id.split(":")[0]) || (yield e)
             }
-            const x = [n.e(7531).then(n.t.bind(n, 7531, 23))],
-                O = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
+            const O = [n.e(7531).then(n.t.bind(n, 7531, 23))],
+                x = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
             window.addEventListener("load", (async function() {
-                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(4319), n(24132), n(41412), n(99661), n(59601), j],
+                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(4319), n(24132), n(41412), n(99661), n(59601), P],
                     t = [n(84632), n(70851)],
                     s = JSON.parse(i.PageConfig.getOption("federated_extensions")),
                     l = [],
-                    c = [],
                     u = [],
+                    c = [],
                     d = [],
                     p = await Promise.allSettled(s.map((async e => (await async function(e, t) {
                         await
                         function(e) {
                             return new Promise(((t, n) => {
                                 const i = document.createElement("script");
                                 i.onerror = n, i.onload = t, i.async = !0, document.head.appendChild(i), i.src = e
@@ -334,34 +324,34 @@
                         }(e), await n.I("default");
                         const i = window._JUPYTERLAB[t];
                         await i.init(n.S.default)
                     }(`${i.URLExt.join(i.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))));
                 Object.entries(p).forEach((([e, t]) => {
                     if ("rejected" === t.status) return void console.error(t.reason);
                     const n = t.value;
-                    n.liteExtension ? d.push(k(n.name, n.extension)) : (n.extension && l.push(k(n.name, n.extension)), n.mimeExtension && c.push(k(n.name, n.mimeExtension)), n.style && u.push(k(n.name, n.style)))
+                    n.liteExtension ? d.push(k(n.name, n.extension)) : (n.extension && l.push(k(n.name, n.extension)), n.mimeExtension && u.push(k(n.name, n.mimeExtension)), n.style && c.push(k(n.name, n.style)))
                 })), (await Promise.allSettled(l)).forEach((t => {
                     if ("fulfilled" === t.status)
-                        for (const n of C(t.value, O)) e.push(n);
+                        for (const n of C(t.value, x)) e.push(n);
                     else console.error(t.reason)
-                })), (await Promise.allSettled(c)).forEach((e => {
+                })), (await Promise.allSettled(u)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (const n of C(e.value, O)) t.push(n);
+                        for (const n of C(e.value, x)) t.push(n);
                     else console.error(e.reason)
-                })), (await Promise.allSettled(u)).filter((({
+                })), (await Promise.allSettled(c)).filter((({
                     status: e
                 }) => "rejected" === e)).forEach((e => {
                     console.error(e.reason)
                 }));
                 const g = [];
-                (await Promise.all(x)).forEach((e => {
-                    for (const t of C(e, O)) g.push(t)
+                (await Promise.all(O)).forEach((e => {
+                    for (const t of C(e, x)) g.push(t)
                 })), (await Promise.allSettled(d)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (const t of C(e.value, O)) g.push(t);
+                        for (const t of C(e.value, x)) g.push(t);
                     else console.error(e.reason)
                 }));
                 const m = new a.JupyterLiteServer({
                     shell: null
                 });
                 m.registerPluginModules(g), await m.start();
                 const h = await m.resolveRequiredService(r.IKernelSpecs),
```

### Comparing `voici-0.4.0/voici/static/build/5826.js` & `voici-0.4.1/voici/static/build/5826.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/5950.js` & `voici-0.4.1/voici/static/build/5950.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,23 @@
+/*! For license information please see 5950.js.LICENSE.txt */
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5950], {
         45950: (e, t, r) => {
             "use strict";
             r.r(t), r.d(t, {
                 MIME_TYPE: () => m,
                 RenderedJSON: () => v,
                 default: () => O,
                 rendererFactory: () => g
             });
             var a = r(37782),
                 n = r(56956),
                 o = r(42051),
                 s = r(97505),
-                i = r(28316),
+                i = r(24627),
                 l = r(24643),
                 u = r(92233),
                 c = r(82701),
                 f = r.n(c),
                 b = r(30650);
             class d extends s.Component {
                 constructor() {
@@ -720,20 +721,20 @@
             t.harmonic = a(k);
             var M = r(3233);
             t.hopscotch = a(M);
             var x = r(41630);
             t.isotope = a(x);
             var C = r(80988);
             t.marrakesh = a(C);
-            var A = r(94793);
-            t.mocha = a(A);
-            var S = r(81762);
-            t.monokai = a(S);
-            var P = r(27172);
-            t.ocean = a(P);
+            var S = r(94793);
+            t.mocha = a(S);
+            var P = r(81762);
+            t.monokai = a(P);
+            var A = r(27172);
+            t.ocean = a(A);
             var R = r(28079);
             t.paraiso = a(R);
             var D = r(48111);
             t.pop = a(D);
             var N = r(34733);
             t.railscasts = a(N);
             var T = r(80133);
@@ -2394,17 +2395,17 @@
                 E = /^\s+|\s+$/g,
                 j = /\{(?:\n\/\* \[wrapped with .+\] \*\/)?\n?/,
                 _ = /\{\n\/\* \[wrapped with (.+)\] \*/,
                 k = /,? & /,
                 M = /^[-+]0x[0-9a-f]+$/i,
                 x = /^0b[01]+$/i,
                 C = /^\[object .+?Constructor\]$/,
-                A = /^0o[0-7]+$/i,
-                S = /^(?:0|[1-9]\d*)$/,
-                P = parseInt,
+                S = /^0o[0-7]+$/i,
+                P = /^(?:0|[1-9]\d*)$/,
+                A = parseInt,
                 R = "object" == typeof r.g && r.g && r.g.Object === Object && r.g,
                 D = "object" == typeof self && self && self.Object === Object && self,
                 N = R || D || Function("return this")();
 
             function T(e, t, r) {
                 switch (r.length) {
                     case 0:
@@ -2566,15 +2567,15 @@
             function oe(e, t) {
                 var r = t.length,
                     a = r - 1;
                 return t[a] = (r > 1 ? "& " : "") + t[a], t = t.join(r > 2 ? ", " : " "), e.replace(j, "{\n/* [wrapped with " + t + "] */\n")
             }
 
             function se(e, t) {
-                return !!(t = null == t ? p : t) && ("number" == typeof e || S.test(e)) && e > -1 && e % 1 == 0 && e < t
+                return !!(t = null == t ? p : t) && ("number" == typeof e || P.test(e)) && e > -1 && e % 1 == 0 && e < t
             }
             var ie = X ? function(e, t, r) {
                 var a, n = t + "";
                 return X(e, "toString", {
                     configurable: !0,
                     enumerable: !1,
                     value: (a = oe(n, le(ne(n), r)), function() {
@@ -2659,22 +2660,57 @@
                             if (ce(e)) {
                                 var t = "function" == typeof e.valueOf ? e.valueOf() : e;
                                 e = ce(t) ? t + "" : t
                             }
                             if ("string" != typeof e) return 0 === e ? e : +e;
                             e = e.replace(E, "");
                             var r = x.test(e);
-                            return r || A.test(e) ? P(e.slice(2), r ? 2 : 8) : M.test(e) ? m : +e
+                            return r || S.test(e) ? A(e.slice(2), r ? 2 : 8) : M.test(e) ? m : +e
                         }(e)) === h || e === -h ? (e < 0 ? -1 : 1) * y : e == e ? e : 0 : 0 === e ? e : 0
                     }(e),
                     r = t % 1;
                 return t == t ? r ? t - r : t : 0
             }
             ue.placeholder = {}, e.exports = ue
         },
+        37320: e => {
+            "use strict";
+            var t = Object.getOwnPropertySymbols,
+                r = Object.prototype.hasOwnProperty,
+                a = Object.prototype.propertyIsEnumerable;
+            e.exports = function() {
+                try {
+                    if (!Object.assign) return !1;
+                    var e = new String("abc");
+                    if (e[5] = "de", "5" === Object.getOwnPropertyNames(e)[0]) return !1;
+                    for (var t = {}, r = 0; r < 10; r++) t["_" + String.fromCharCode(r)] = r;
+                    if ("0123456789" !== Object.getOwnPropertyNames(t).map((function(e) {
+                            return t[e]
+                        })).join("")) return !1;
+                    var a = {};
+                    return "abcdefghijklmnopqrst".split("").forEach((function(e) {
+                        a[e] = e
+                    })), "abcdefghijklmnopqrst" === Object.keys(Object.assign({}, a)).join("")
+                } catch (e) {
+                    return !1
+                }
+            }() ? Object.assign : function(e, n) {
+                for (var o, s, i = function(e) {
+                        if (null == e) throw new TypeError("Object.assign cannot be called with null or undefined");
+                        return Object(e)
+                    }(e), l = 1; l < arguments.length; l++) {
+                    for (var u in o = Object(arguments[l])) r.call(o, u) && (i[u] = o[u]);
+                    if (t) {
+                        s = t(o);
+                        for (var c = 0; c < s.length; c++) a.call(o, s[c]) && (i[s[c]] = o[s[c]])
+                    }
+                }
+                return i
+            }
+        },
         68262: (e, t, r) => {
             "use strict";
             var a = r(23586);
 
             function n() {}
 
             function o() {}
```

### Comparing `voici-0.4.0/voici/static/build/5952.js` & `voici-0.4.1/voici/static/build/5952.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/596.js` & `voici-0.4.1/voici/static/build/596.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/5985.js` & `voici-0.4.1/voici/static/build/5985.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6111.js` & `voici-0.4.1/voici/static/build/6111.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6178.js` & `voici-0.4.1/voici/static/build/6178.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6196.js` & `voici-0.4.1/voici/static/build/6196.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6219.js` & `voici-0.4.1/voici/static/build/6219.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6219.js.LICENSE.txt` & `voici-0.4.1/voici/static/build/6219.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6527.js` & `voici-0.4.1/voici/static/build/6527.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6614.js` & `voici-0.4.1/voici/static/build/6614.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6616.js` & `voici-0.4.1/voici/static/build/6616.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6757.js` & `voici-0.4.1/voici/static/build/6757.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6770.js` & `voici-0.4.1/voici/static/build/6770.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6790.js` & `voici-0.4.1/voici/static/build/6790.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6839.js` & `voici-0.4.1/voici/static/build/6839.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6852.js` & `voici-0.4.1/voici/static/build/6852.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6852], {
         27693: e => {
             e.exports = {
                 name: "@voila-dashboards/voici",
-                version: "0.4.0",
+                version: "0.4.1",
                 description: "The Voici Frontend",
                 author: "Voilà contributors",
                 license: "BSD-3-Clause",
                 main: "lib/index.js",
                 browserslist: ">0.8%, not ie 11, not op_mini all, not dead",
                 dependencies: {
                     "@jupyter-widgets/base": "^6.0.1",
@@ -49,15 +49,16 @@
                     "@lumino/dragdrop": "^1.10.2",
                     "@lumino/messaging": "^1.7.2",
                     "@lumino/properties": "^1.5.2",
                     "@lumino/signaling": "^1.7.2",
                     "@lumino/virtualdom": "^1.11.2",
                     "@lumino/widgets": "^1.26.2",
                     "@voila-dashboards/voila": "^0.5.0-alpha.3",
-                    react: "^17.0.1"
+                    react: "^17.0.1",
+                    "react-dom": "^17.0.1"
                 },
                 devDependencies: {
                     "@babel/core": "^7.2.2",
                     "@babel/preset-env": "^7.3.1",
                     "@jupyterlab/builder": "^3.0.0",
                     "@types/node": "^18.8.3",
                     "babel-loader": "^8.0.5",
@@ -97,31 +98,31 @@
             }
         },
         46852: (e, t, n) => {
             "use strict";
             n.r(t), n(71024);
             var i = n(59110),
                 a = n(94456),
-                o = n(22312),
-                r = n(75238),
+                r = n(22312),
+                o = n(75238),
                 s = n(73198),
                 l = n(40049),
                 u = n(12299),
                 c = n(35918),
                 d = n(92233),
                 p = n(42051);
             const g = n(27693),
                 m = "application/vnd.jupyter.widget-view+json";
-            class h extends r.JupyterFrontEnd {
+            class h extends o.JupyterFrontEnd {
                 constructor(e) {
                     var t;
                     if (super(Object.assign(Object.assign({}, e), {
-                            shell: null !== (t = e.shell) && void 0 !== t ? t : new o.VoilaShell
+                            shell: null !== (t = e.shell) && void 0 !== t ? t : new r.VoilaShell
                         })), this.name = "Voici", this.namespace = this.name, this.version = g.version, this._widgetManagerPromise = new d.PromiseDelegate, e.mimeExtensions)
-                        for (const t of (0, r.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
+                        for (const t of (0, o.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
                     this._kernelspecs = e.kernelspecs, this._serviceManager = e.serviceManager
                 }
                 get widgetManagerPromise() {
                     return this._widgetManagerPromise
                 }
                 get paths() {
                     return {
@@ -167,33 +168,33 @@
                     }))
                 }
                 async renderWidgets() {
                     var e, t, n;
                     const a = this._serviceManager;
                     if (!a) return void console.error("Missing service manager");
                     await a.ready;
-                    const o = a.sessions;
-                    await o.ready;
-                    const r = new l.NotebookModel;
-                    r.fromString(i.PageConfig.getOption("notebookSrc"));
-                    let s = r.metadata.get("kernelspec");
+                    const r = a.sessions;
+                    await r.ready;
+                    const o = new l.NotebookModel;
+                    o.fromString(i.PageConfig.getOption("notebookSrc"));
+                    let s = o.metadata.get("kernelspec");
                     s || (s = {
                         name: "python"
                     });
                     const d = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
                     let p;
                     if (!d) return void console.error("No kernel available");
                     if (s.name in d) console.log(`${s.name} kernel is available!`), p = d[s.name];
                     else
                         for (const e in d)
                             if (s.language === (null === (n = d[e]) || void 0 === n ? void 0 : n.language)) {
                                 console.log(`${s.name} kernel is not available, fallback to using ${d[e].name}`), p = d[e];
                                 break
                             } if (!p) return void console.error(`No kernel available for ${s.language}`);
-                    const g = await o.startNew({
+                    const g = await r.startNew({
                             name: "",
                             path: "",
                             type: "notebook",
                             kernel: p
                         }),
                         h = g.kernel;
                     h ? h.connectionStatusChanged.connect((async (e, t) => {
@@ -206,86 +207,75 @@
                             if (e.removeMimeType(m), e.addFactory({
                                     safe: !1,
                                     mimeTypes: [m],
                                     createRenderer: e => new c.WidgetRenderer(e, t)
                                 }, -10), this._widgetManagerPromise.resolve(t), !g.kernel) return;
                             await new Promise((e => setTimeout(e, 500)));
                             let n = !1;
-                            const a = i.PageConfig.getOption("packagesSrc");
                             h.statusChanged.connect((async (t, i) => {
                                 n || "idle" !== i || (n = !0, await b.executeCells({
-                                    packages: a,
-                                    source: r,
+                                    source: o,
                                     rendermime: e,
                                     kernel: g.kernel
                                 }))
                             }))
                         }
                     })) : console.error("Can not start kernel")
                 }
             }
             var b;
             ! function(e) {
                 e.executeCells = async function(e) {
                     var t, n;
                     const {
-                        packages: i,
-                        source: a,
-                        rendermime: o,
+                        source: i,
+                        rendermime: a,
                         kernel: r
-                    } = e;
-                    if (i && i.length > 0) {
-                        window.update_loading_text(0, 0, "Installing dependencies");
-                        const e = r.requestExecute({
-                            code: i
-                        });
-                        await e.done
-                    }
-                    const l = a.cells.length;
-                    for (let e = 0; e < l; e++) {
-                        const i = a.cells.get(e);
-                        if (window.update_loading_text(e + 1, l, null), "code" !== i.type) {
-                            e === l - 1 && window.display_cells();
+                    } = e, o = i.cells.length;
+                    for (let e = 0; e < o; e++) {
+                        const l = i.cells.get(e);
+                        if (window.update_loading_text(e + 1, o, null), "code" !== l.type) {
+                            e === o - 1 && window.display_cells();
                             continue
                         }
                         const u = new s.OutputAreaModel({
                                 trusted: !0
                             }),
                             c = new s.SimplifiedOutputArea({
                                 model: u,
-                                rendermime: o
+                                rendermime: a
                             });
                         c.future = r.requestExecute({
-                            code: i.value.text
+                            code: l.value.text
                         }), await c.future.done;
                         const d = document.querySelector(`[cell-index="${e+1}"]`);
                         if (d && c.node.childNodes.length > 0) {
                             null === (t = d.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
                             const e = document.createElement("div");
                             e.classList.add("jp-Cell-outputWrapper"), null === (n = d.lastElementChild) || void 0 === n || n.appendChild(e), c.node.classList.add("jp-Cell-outputArea", "jp-OutputArea-child"), p.Widget.attach(c, e)
                         }
-                        e === l - 1 && (window.display_cells(), window.dispatchEvent(new Event("resize")))
+                        e === o - 1 && (window.display_cells(), window.dispatchEvent(new Event("resize")))
                     }
                 }
             }(b || (b = {}));
             var f = n(67651),
                 y = n(37782);
             f.IJupyterWidgetRegistry;
             const w = {
                 id: "@voila-dashboards/voici:theme-manager",
                 autoStart: !0,
                 optional: [y.IThemeManager],
                 activate: (e, t) => {
                     if (!t) return;
                     const n = window.location.search,
                         a = new URLSearchParams(n).get("theme"),
-                        o = i.PageConfig.getOption("jpThemeName");
-                    let r = a ? decodeURIComponent(a) : o;
-                    r = r || "light", "dark" !== r && "JupyterLab Dark" !== r || (r = "JupyterLab Dark"), "light" !== r && "JupyterLab Light" !== r || (r = "JupyterLab Light"), t.themeChanged.connect((() => {
-                        t.theme !== r && t.setTheme(r)
+                        r = i.PageConfig.getOption("jpThemeName");
+                    let o = a ? decodeURIComponent(a) : r;
+                    o = o || "light", "dark" !== o && "JupyterLab Dark" !== o || (o = "JupyterLab Dark"), "light" !== o && "JupyterLab Light" !== o || (o = "JupyterLab Light"), t.themeChanged.connect((() => {
+                        t.theme !== o && t.setTheme(o)
                     }))
                 }
             };
             async function v(e, t) {
                 try {
                     return (await window._JUPYTERLAB[e].get(t))()
                 } catch (n) {
@@ -295,25 +285,25 @@
 
             function* P(e, t) {
                 let n;
                 n = Object.prototype.hasOwnProperty.call(e, "__esModule") ? e.default : e;
                 const a = Array.isArray(n) ? n : [n];
                 for (const e of a) i.PageConfig.Extension.isDisabled(e.id) || t.includes(e.id) || t.includes(e.id.split(":")[0]) || (yield e)
             }
-            o.pathsPlugin, o.translatorPlugin;
+            r.pathsPlugin, r.translatorPlugin;
             const j = [n.e(7531).then(n.t.bind(n, 7531, 23))],
-                k = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
+                C = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
             window.addEventListener("load", (async function() {
-                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(99661), n(59601), o.translatorPlugin, o.pathsPlugin, w],
+                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(99661), n(59601), r.translatorPlugin, r.pathsPlugin, w],
                     t = [],
-                    r = JSON.parse(i.PageConfig.getOption("federated_extensions")),
+                    o = JSON.parse(i.PageConfig.getOption("federated_extensions")),
                     s = [],
                     l = [],
                     u = [],
-                    c = await Promise.allSettled(r.map((async e => (await async function(e, t) {
+                    c = await Promise.allSettled(o.map((async e => (await async function(e, t) {
                         await
                         function(e) {
                             return new Promise(((t, n) => {
                                 const i = document.createElement("script");
                                 i.onerror = n, i.onload = t, i.async = !0, document.head.appendChild(i), i.src = e
                             }))
                         }(e), await n.I("default");
@@ -322,37 +312,37 @@
                     }(`${i.URLExt.join(i.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))));
                 Object.entries(c).forEach((([e, t]) => {
                     if ("rejected" === t.status) return void console.error(t.reason);
                     const n = t.value;
                     n.extension && s.push(v(n.name, n.extension)), n.mimeExtension && l.push(v(n.name, n.mimeExtension)), n.style && u.push(v(n.name, n.style))
                 })), (await Promise.allSettled(s)).forEach((t => {
                     if ("fulfilled" === t.status)
-                        for (const n of P(t.value, k)) e.push(n);
+                        for (const n of P(t.value, C)) e.push(n);
                     else console.error(t.reason)
                 })), (await Promise.allSettled(l)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (const n of P(e.value, k)) t.push(n);
+                        for (const n of P(e.value, C)) t.push(n);
                     else console.error(e.reason)
                 })), (await Promise.allSettled(u)).filter((({
                     status: e
                 }) => "rejected" === e)).forEach((e => {
                     console.error(e.reason)
                 }));
                 const d = [];
                 (await Promise.all(j)).forEach((e => {
-                    for (const t of P(e, k)) d.push(t)
+                    for (const t of P(e, C)) d.push(t)
                 }));
                 const p = new a.JupyterLiteServer({
                     shell: null
                 });
                 p.registerPluginModules(d), await p.start();
                 const g = p.serviceManager,
                     m = new h({
                         serviceManager: g,
-                        shell: new o.VoilaShell
+                        shell: new r.VoilaShell
                     });
                 m.registerPluginModules(e), m.started.then((() => {
                     const e = document.getElementById("voila-tree-main");
                     e && (e.style.display = "unset")
                 })), m.start()
             }))
         }
```

### Comparing `voici-0.4.0/voici/static/build/6856.js` & `voici-0.4.1/voici/static/build/6856.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6914.js` & `voici-0.4.1/voici/static/build/6914.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/6976.js` & `voici-0.4.1/voici/static/build/6976.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/7003.js` & `voici-0.4.1/voici/static/build/7003.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/7015.js` & `voici-0.4.1/voici/static/build/7015.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/7066.js` & `voici-0.4.1/voici/static/build/7066.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -188,15 +188,15 @@
                             }
                         }
                     }))
                 }
             };
             var b = a(84939),
                 v = a(97505),
-                _ = a(28316);
+                _ = a(24627);
             const w = "jp-Notification-Toast-Close";
             var C;
 
             function k(e) {
                 const {
                     manager: t,
                     onClose: a,
```

### Comparing `voici-0.4.0/voici/static/build/709.js` & `voici-0.4.1/voici/static/build/709.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/74.js` & `voici-0.4.1/voici/static/build/74.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/7469.js` & `voici-0.4.1/voici/static/build/7469.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/7560.js` & `voici-0.4.1/voici/static/build/7560.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/7623.js` & `voici-0.4.1/voici/static/build/7623.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/7695.js` & `voici-0.4.1/voici/static/build/7695.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/7795.js` & `voici-0.4.1/voici/static/build/7795.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/8085.js` & `voici-0.4.1/voici/static/build/8085.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/8164.js` & `voici-0.4.1/voici/static/build/8164.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/8291.js` & `voici-0.4.1/voici/static/build/8291.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/8316.js` & `voici-0.4.1/voici/static/build/8316.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/8316.js.LICENSE.txt` & `voici-0.4.1/voici/static/build/8316.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/846.js` & `voici-0.4.1/voici/static/build/846.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/86.js` & `voici-0.4.1/voici/static/build/86.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/8809.js` & `voici-0.4.1/voici/static/build/8809.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/8874.js` & `voici-0.4.1/voici/static/build/8874.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9060.js` & `voici-0.4.1/voici/static/build/9060.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9112.js` & `voici-0.4.1/voici/static/build/9112.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9339.js` & `voici-0.4.1/voici/static/build/9339.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9406.js` & `voici-0.4.1/voici/static/build/9406.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9513.js` & `voici-0.4.1/voici/static/build/9513.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9727.js` & `voici-0.4.1/voici/static/build/9727.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9757.js` & `voici-0.4.1/voici/static/build/9757.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9780.js` & `voici-0.4.1/voici/static/build/9780.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9807.js` & `voici-0.4.1/voici/static/build/9807.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9900.js` & `voici-0.4.1/voici/static/build/9900.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/9988.js` & `voici-0.4.1/voici/static/build/9988.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/service-worker-b2fb40a.js` & `voici-0.4.1/voici/static/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/voici/static/build/treepage.js` & `voici-0.4.1/voici/static/build/treepage.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                         (!i || !i.loaded && (!r != !i.eager ? r : o > i.from)) && (a[t] = {
                             get: l,
                             from: o,
                             eager: !!r
                         })
                     },
                     u = [];
-                return "default" === l && (i("@jupyter-widgets/base", "6.0.4", (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))), i("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([c.e(8291), c.e(3851), c.e(4947), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(7651), c.e(6587)]).then((() => () => c(53851))))), i("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(988), c.e(2299), c.e(8930), c.e(3198), c.e(7651), c.e(49), c.e(5320), c.e(6678), c.e(2266)]).then((() => () => c(9727))))), i("@jupyter-widgets/output", "6.0.4", (() => Promise.all([c.e(7651), c.e(1100)]).then((() => () => c(21100))))), i("@jupyterlab/application", "3.6.3", (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))), i("@jupyterlab/apputils-extension", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(8316), c.e(7066), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(7505), c.e(1514), c.e(7968), c.e(8930), c.e(5238), c.e(5320)]).then((() => () => c(97066))))), i("@jupyterlab/apputils", "3.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(8316), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(988), c.e(7505), c.e(8695), c.e(1514), c.e(4812), c.e(8930), c.e(1732)]).then((() => () => c(90339))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(286), c.e(4947), c.e(2233), c.e(6616)]).then((() => () => c(20286))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(2233), c.e(709)]).then((() => () => c(62359))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(2233), c.e(6178)]).then((() => () => c(70053))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(3922), c.e(4947), c.e(2233), c.e(2630)]).then((() => () => c(13922))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(2233), c.e(6614)]).then((() => () => c(20596))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(2233), c.e(1023)]).then((() => () => c(1980))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(2233), c.e(6790)]).then((() => () => c(4896))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(2233), c.e(3086)]).then((() => () => c(60103))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(2950), c.e(4947), c.e(2233), c.e(1667)]).then((() => () => c(42950))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(3251), c.e(4947), c.e(2233), c.e(7623)]).then((() => () => c(53251))))), i("@jupyterlab/docregistry", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(2299), c.e(7505), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))), i("@jupyterlab/json-extension", "3.6.3", (() => Promise.all([c.e(8316), c.e(5950), c.e(2233), c.e(6956), c.e(2051), c.e(7782), c.e(4643), c.e(7505)]).then((() => () => c(45950))))), i("@jupyterlab/logconsole", "3.6.3", (() => Promise.all([c.e(9339), c.e(4947), c.e(2233), c.e(6956), c.e(2051), c.e(2299), c.e(3198)]).then((() => () => c(99339))))), i("@jupyterlab/mainmenu", "3.6.3", (() => Promise.all([c.e(2233), c.e(3203), c.e(2051), c.e(4643), c.e(1581)]).then((() => () => c(21581))))), i("@jupyterlab/markdownviewer-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(2299), c.e(7968), c.e(8930), c.e(5238), c.e(4382)]).then((() => () => c(54382))))), i("@jupyterlab/mathjax2-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(9110), c.e(2299), c.e(6976)]).then((() => () => c(66976))))), i("@jupyterlab/nbformat", "3.6.3", (() => Promise.all([c.e(2233), c.e(3655)]).then((() => () => c(63655))))), i("@jupyterlab/notebook", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(7505), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(3198), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))), i("@jupyterlab/outputarea", "3.6.3", (() => Promise.all([c.e(1432), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(4629), c.e(7782), c.e(988), c.e(2299), c.e(9939)]).then((() => () => c(31432))))), i("@jupyterlab/rendermime-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(7782), c.e(2299), c.e(5985)]).then((() => () => c(85985))))), i("@jupyterlab/rendermime", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(846), c.e(7560), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9098), c.e(3008)]).then((() => () => c(17560))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(74), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9320)]).then((() => () => c(80074))))), i("@jupyterlab/services", "6.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9110), c.e(1497)]).then((() => () => c(16914))))), i("@jupyterlab/settingregistry", "3.6.3", (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(2233), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))), i("@jupyterlab/theme-dark-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(1058)]).then((() => () => c(21058))))), i("@jupyterlab/theme-light-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(275)]).then((() => () => c(60275))))), i("@jupyterlab/translation", "3.6.3", (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))), i("@jupyterlab/ui-components", "3.6.3", (() => Promise.all([c.e(6770), c.e(8316), c.e(4963), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7505), c.e(2886)]).then((() => () => c(74963))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([c.e(9757), c.e(2233), c.e(9110)]).then((() => () => c(9757))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([c.e(2233), c.e(2051), c.e(6527)]).then((() => () => c(26527))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(2233), c.e(5820)]).then((() => () => c(83693))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([c.e(6111), c.e(4530), c.e(2233), c.e(3203), c.e(4456), c.e(7631), c.e(3862)]).then((() => () => c(24530))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2233), c.e(2051), c.e(1514), c.e(568), c.e(3256)]).then((() => () => c(93256))))), i("@lumino/algorithm", "1.9.2", (() => c.e(9060).then((() => () => c(69060))))), i("@lumino/algorithm", "2.0.0", (() => c.e(9807).then((() => () => c(89807))))), i("@lumino/commands", "1.21.1", (() => Promise.all([c.e(2687), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))), i("@lumino/coreutils", "1.12.1", (() => c.e(1770).then((() => () => c(71770))))), i("@lumino/coreutils", "2.1.0", (() => c.e(4259).then((() => () => c(4259))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))), i("@lumino/domutils", "1.8.2", (() => c.e(5403).then((() => () => c(85403))))), i("@lumino/dragdrop", "1.14.5", (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))), i("@lumino/properties", "1.8.2", (() => c.e(3312).then((() => () => c(73312))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))), i("@lumino/signaling", "2.1.0", (() => Promise.all([c.e(6088), c.e(319), c.e(7003)]).then((() => () => c(27003))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([c.e(1053), c.e(3203)]).then((() => () => c(1053))))), i("@lumino/widgets", "1.37.2", (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))), i("@voila-dashboards/voila", "0.5.0-alpha.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(988), c.e(2299), c.e(7651), c.e(5238), c.e(5918), c.e(3504)]).then((() => () => c(17696))))), i("react", "17.0.2", (() => c.e(2784).then((() => () => c(2784)))))), e[l] = u.length ? Promise.all(u).then((() => e[l] = 1)) : 1
+                return "default" === l && (i("@jupyter-widgets/base", "6.0.4", (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))), i("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([c.e(8291), c.e(3851), c.e(4947), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(7651), c.e(6587)]).then((() => () => c(53851))))), i("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(988), c.e(2299), c.e(8930), c.e(3198), c.e(7651), c.e(49), c.e(5320), c.e(6678), c.e(2266)]).then((() => () => c(9727))))), i("@jupyter-widgets/output", "6.0.4", (() => Promise.all([c.e(7651), c.e(1100)]).then((() => () => c(21100))))), i("@jupyterlab/application", "3.6.3", (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))), i("@jupyterlab/apputils-extension", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5238), c.e(5320)]).then((() => () => c(97066))))), i("@jupyterlab/apputils", "3.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(1514), c.e(4812), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(286), c.e(4947), c.e(2233), c.e(6616)]).then((() => () => c(20286))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(2233), c.e(709)]).then((() => () => c(62359))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(2233), c.e(6178)]).then((() => () => c(70053))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(3922), c.e(4947), c.e(2233), c.e(2630)]).then((() => () => c(13922))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(2233), c.e(6614)]).then((() => () => c(20596))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(2233), c.e(1023)]).then((() => () => c(1980))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(2233), c.e(6790)]).then((() => () => c(4896))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(2233), c.e(3086)]).then((() => () => c(60103))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(2950), c.e(4947), c.e(2233), c.e(1667)]).then((() => () => c(42950))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(3251), c.e(4947), c.e(2233), c.e(7623)]).then((() => () => c(53251))))), i("@jupyterlab/docregistry", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(2299), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))), i("@jupyterlab/json-extension", "3.6.3", (() => Promise.all([c.e(5950), c.e(2233), c.e(6956), c.e(2051), c.e(7782), c.e(4643), c.e(7505), c.e(4627)]).then((() => () => c(45950))))), i("@jupyterlab/logconsole", "3.6.3", (() => Promise.all([c.e(9339), c.e(4947), c.e(2233), c.e(6956), c.e(2051), c.e(2299), c.e(3198)]).then((() => () => c(99339))))), i("@jupyterlab/mainmenu", "3.6.3", (() => Promise.all([c.e(2233), c.e(3203), c.e(2051), c.e(4643), c.e(1581)]).then((() => () => c(21581))))), i("@jupyterlab/markdownviewer-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(2299), c.e(7968), c.e(8930), c.e(5238), c.e(4382)]).then((() => () => c(54382))))), i("@jupyterlab/mathjax2-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(9110), c.e(2299), c.e(6976)]).then((() => () => c(66976))))), i("@jupyterlab/nbformat", "3.6.3", (() => Promise.all([c.e(2233), c.e(3655)]).then((() => () => c(63655))))), i("@jupyterlab/notebook", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(2299), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(3198), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))), i("@jupyterlab/outputarea", "3.6.3", (() => Promise.all([c.e(1432), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(4629), c.e(7782), c.e(988), c.e(2299), c.e(9939)]).then((() => () => c(31432))))), i("@jupyterlab/rendermime-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(7782), c.e(2299), c.e(5985)]).then((() => () => c(85985))))), i("@jupyterlab/rendermime", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(846), c.e(7560), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9098), c.e(3008)]).then((() => () => c(17560))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(74), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9320)]).then((() => () => c(80074))))), i("@jupyterlab/services", "6.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9110), c.e(1497)]).then((() => () => c(16914))))), i("@jupyterlab/settingregistry", "3.6.3", (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(2233), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))), i("@jupyterlab/theme-dark-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(1058)]).then((() => () => c(21058))))), i("@jupyterlab/theme-light-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(275)]).then((() => () => c(60275))))), i("@jupyterlab/translation", "3.6.3", (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))), i("@jupyterlab/ui-components", "3.6.3", (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([c.e(9757), c.e(2233), c.e(9110)]).then((() => () => c(9757))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([c.e(2233), c.e(2051), c.e(6527)]).then((() => () => c(26527))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(2233), c.e(5820)]).then((() => () => c(83693))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([c.e(6111), c.e(4530), c.e(2233), c.e(3203), c.e(4456), c.e(7631), c.e(3862)]).then((() => () => c(24530))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2233), c.e(2051), c.e(1514), c.e(568), c.e(3256)]).then((() => () => c(93256))))), i("@lumino/algorithm", "1.9.2", (() => c.e(9060).then((() => () => c(69060))))), i("@lumino/algorithm", "2.0.0", (() => c.e(9807).then((() => () => c(89807))))), i("@lumino/commands", "1.21.1", (() => Promise.all([c.e(2687), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))), i("@lumino/coreutils", "1.12.1", (() => c.e(1770).then((() => () => c(71770))))), i("@lumino/coreutils", "2.1.0", (() => c.e(4259).then((() => () => c(4259))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))), i("@lumino/domutils", "1.8.2", (() => c.e(5403).then((() => () => c(85403))))), i("@lumino/dragdrop", "1.14.5", (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))), i("@lumino/properties", "1.8.2", (() => c.e(3312).then((() => () => c(73312))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))), i("@lumino/signaling", "2.1.0", (() => Promise.all([c.e(6088), c.e(319), c.e(7003)]).then((() => () => c(27003))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([c.e(1053), c.e(3203)]).then((() => () => c(1053))))), i("@lumino/widgets", "1.37.2", (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))), i("@voila-dashboards/voila", "0.5.0-alpha.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(988), c.e(2299), c.e(7651), c.e(5238), c.e(5918), c.e(3504)]).then((() => () => c(17696))))), i("react-dom", "17.0.2", (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))), i("react", "17.0.2", (() => c.e(2784).then((() => () => c(2784)))))), e[l] = u.length ? Promise.all(u).then((() => e[l] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         c.g.importScripts && (e = c.g.location + "");
         var t = c.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
@@ -196,24 +196,25 @@
         36e3: () => s("default", "@lumino/disposable", [1, 1, 7, 2], (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))),
         56956: () => s("default", "@jupyterlab/translation", [1, 3, 0, 0], (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))),
         24629: () => s("default", "@lumino/properties", [1, 1, 5, 2], (() => c.e(3312).then((() => () => c(73312))))),
         70988: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(3203), c.e(6e3), c.e(9110), c.e(6417)]).then((() => () => c(16914))))),
         12299: () => s("default", "@jupyterlab/rendermime", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))),
         68930: () => s("default", "@jupyterlab/settingregistry", [1, 3, 0, 0], (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))),
         73198: () => s("default", "@jupyterlab/outputarea", [1, 3, 0, 0], (() => Promise.all([c.e(1432), c.e(4947), c.e(3203), c.e(4629), c.e(7782), c.e(988), c.e(9939)]).then((() => () => c(31432))))),
-        40049: () => s("default", "@jupyterlab/notebook", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(7505), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))),
+        40049: () => s("default", "@jupyterlab/notebook", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))),
         5320: () => s("default", "@jupyterlab/mainmenu", [1, 3, 0, 0], (() => Promise.all([c.e(4643), c.e(9406)]).then((() => () => c(21581))))),
         10409: () => s("default", "@jupyter-widgets/output", [1, 6, 0, 1], (() => c.e(7015).then((() => () => c(21100))))),
         70190: () => s("default", "@jupyterlab/logconsole", [1, 3, 0, 0], (() => c.e(9339).then((() => () => c(99339))))),
         59110: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(6196)]).then((() => () => c(60103))))),
-        37782: () => s("default", "@jupyterlab/apputils", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(846), c.e(8316), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(988), c.e(7505), c.e(8695), c.e(1514), c.e(4812), c.e(8930), c.e(1732)]).then((() => () => c(90339))))),
-        24643: () => s("default", "@jupyterlab/ui-components", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(8316), c.e(4963), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(9110), c.e(7505), c.e(2886)]).then((() => () => c(74963))))),
+        37782: () => s("default", "@jupyterlab/apputils", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(1514), c.e(4812), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))),
+        24643: () => s("default", "@jupyterlab/ui-components", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))),
         1514: () => s("default", "@lumino/commands", [1, 1, 15, 2], (() => Promise.all([c.e(2687), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))),
-        77968: () => s("default", "@jupyterlab/docregistry", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(3203), c.e(6e3), c.e(4643), c.e(2299), c.e(7505), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))),
+        77968: () => s("default", "@jupyterlab/docregistry", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(3203), c.e(6e3), c.e(4643), c.e(7505), c.e(2299), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))),
         97505: () => s("default", "react", [1, 17, 0, 1], (() => c.e(2784).then((() => () => c(2784))))),
+        24627: () => s("default", "react-dom", [1, 17, 0, 1], (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))),
         75238: () => s("default", "@jupyterlab/application", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))),
         56088: () => s("default", "@lumino/coreutils", [1, 1, 8, 2], (() => c.e(4259).then((() => () => c(4259))))),
         91876: () => s("default", "@lumino/signaling", [1, 1, 7, 2], (() => Promise.all([c.e(319), c.e(1553)]).then((() => () => c(27003))))),
         49939: () => s("default", "@jupyterlab/nbformat", [1, 3, 0, 0], (() => c.e(86).then((() => () => c(63655))))),
         32886: () => s("default", "@lumino/virtualdom", [1, 1, 11, 2], (() => c.e(1053).then((() => () => c(1053))))),
         3860: () => s("default", "@lumino/dragdrop", [1, 1, 10, 2], (() => c.e(8809).then((() => () => c(38809))))),
         89098: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(2950), c.e(1105)]).then((() => () => c(42950))))),
@@ -228,15 +229,15 @@
         70771: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(6839)]).then((() => () => c(62359))))),
         81298: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(7795)]).then((() => () => c(20596))))),
         91491: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(5291)]).then((() => () => c(4896))))),
         2132: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(74), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9817)]).then((() => () => c(80074))))),
         86086: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(3922), c.e(8874)]).then((() => () => c(13922))))),
         90319: () => s("default", "@lumino/algorithm", [1, 1, 6, 2], (() => c.e(9807).then((() => () => c(89807))))),
         35918: () => s("default", "@jupyter-widgets/jupyterlab-manager", [1, 5, 0, 3], (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(988), c.e(8930), c.e(3198), c.e(49), c.e(5320), c.e(6678), c.e(2516)]).then((() => () => c(9727))))),
-        9961: () => s("default", "@jupyterlab/apputils-extension", [1, 3, 4, 8], (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(8316), c.e(7066), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(4643), c.e(988), c.e(7505), c.e(1514), c.e(7968), c.e(8930), c.e(5320)]).then((() => () => c(97066))))),
+        9961: () => s("default", "@jupyterlab/apputils-extension", [1, 3, 4, 8], (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5320)]).then((() => () => c(97066))))),
         22312: () => s("default", "@voila-dashboards/voila", [2, 0, 5, 0, , "alpha", 3], (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(988), c.e(2230)]).then((() => () => c(17696))))),
         59601: () => s("default", "@jupyterlab/theme-dark-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6956), c.e(3811)]).then((() => () => c(21058))))),
         99661: () => s("default", "@jupyterlab/theme-light-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6956), c.e(7469)]).then((() => () => c(60275))))),
         17021: () => s("default", "@jupyter-widgets/controls", [1, 5, 0, 1], (() => Promise.all([c.e(3851), c.e(8695), c.e(4812)]).then((() => () => c(53851))))),
         7531: () => s("default", "@jupyterlite/server-extension", [2, 0, 1, 0], (() => Promise.all([c.e(6111), c.e(4530), c.e(3203), c.e(7631), c.e(3862)]).then((() => () => c(24530)))))
     }, h = {
         49: [40049],
@@ -250,14 +251,15 @@
         2299: [12299],
         2886: [32886],
         3198: [73198],
         3203: [23203],
         3860: [3860],
         3862: [48753, 52329, 52390, 70771, 81298, 91491],
         4456: [94456],
+        4627: [24627],
         4629: [24629],
         4643: [24643],
         4812: [94812],
         4863: [17021],
         4947: [4947],
         5238: [75238],
         5320: [5320],
@@ -304,15 +306,15 @@
         var e = {
             9749: 0
         };
         c.f.j = (t, l) => {
             var r = c.o(e, t) ? e[t] : void 0;
             if (0 !== r)
                 if (r) l.push(r[2]);
-                else if (/^(2(051|233|299|886)|3(19(|8)|86[02]|203)|4(456|629|643|812|863|9|947)|5((23|6|91)8|(32|49|82)0)|6(000|088|678|956)|7((53|63|65)1|505|782|968)|8(695|930|987)|9(098|110|88|939)|1514|1876)$/.test(t)) e[t] = 0;
+                else if (/^(2(051|233|299|886)|3(19(|8)|86[02]|203)|4(6(27|29|43)|456|812|863|9|947)|5((23|6|91)8|(32|49|82)0)|6(000|088|678|956)|7((53|63|65)1|505|782|968)|8(695|930|987)|9(098|110|88|939)|1514|1876)$/.test(t)) e[t] = 0;
             else {
                 var a = new Promise(((l, a) => r = e[t] = [l, a]));
                 l.push(r[2] = a);
                 var n = c.p + c.u(t),
                     o = new Error;
                 c.l(n, (l => {
                     if (c.o(e, t) && (0 !== (r = e[t]) && (e[t] = void 0), r)) {
```

### Comparing `voici-0.4.0/voici/static/build/voici.js` & `voici-0.4.1/voici/static/build/voici.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 var _JUPYTERLAB;
 (() => {
-    var e, t, l, r, a, n, o, i, u, s, m, p, h, d = {
+    var e, t, l, r, a, n, o, i, u, s, m, h, p, d = {
             37559: (e, t, l) => {
                 "use strict";
-                Promise.all([l.e(1024), l.e(2233), l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(7631), l.e(5918), l.e(8987), l.e(5474)]).then(l.bind(l, 65474))
+                Promise.all([l.e(1024), l.e(2233), l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(4627), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(7631), l.e(5918), l.e(8987), l.e(5474)]).then(l.bind(l, 65474))
             },
             68444: (e, t, l) => {
                 l.p = function(e) {
                     let t = Object.create(null);
                     if ("undefined" != typeof document && document) {
                         const e = document.getElementById("jupyter-config-data");
                         e && (t = JSON.parse(e.textContent || "{}"))
@@ -67,24 +67,24 @@
                     var m = u[s];
                     if (m.getAttribute("src") == e || m.getAttribute("data-webpack") == r + a) {
                         o = m;
                         break
                     }
                 }
             o || (i = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, c.nc && o.setAttribute("nonce", c.nc), o.setAttribute("data-webpack", r + a), o.src = e), l[e] = [t];
-            var p = (t, r) => {
-                    o.onerror = o.onload = null, clearTimeout(h);
+            var h = (t, r) => {
+                    o.onerror = o.onload = null, clearTimeout(p);
                     var a = l[e];
                     if (delete l[e], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(r))), t) return t(r)
                 },
-                h = setTimeout(p.bind(null, void 0, {
+                p = setTimeout(h.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = p.bind(null, o.onerror), o.onload = p.bind(null, o.onload), i && document.head.appendChild(o)
+            o.onerror = h.bind(null, o.onerror), o.onload = h.bind(null, o.onload), i && document.head.appendChild(o)
         }
     }, c.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                         (!i || !i.loaded && (!r != !i.eager ? r : o > i.from)) && (a[t] = {
                             get: l,
                             from: o,
                             eager: !!r
                         })
                     },
                     u = [];
-                return "default" === l && (i("@jupyter-widgets/base", "6.0.4", (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))), i("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([c.e(8291), c.e(3851), c.e(4947), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(7651), c.e(6587)]).then((() => () => c(53851))))), i("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(988), c.e(2299), c.e(8930), c.e(3198), c.e(7651), c.e(49), c.e(5320), c.e(6678), c.e(2266)]).then((() => () => c(9727))))), i("@jupyter-widgets/output", "6.0.4", (() => Promise.all([c.e(7651), c.e(1100)]).then((() => () => c(21100))))), i("@jupyterlab/application", "3.6.3", (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))), i("@jupyterlab/apputils-extension", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(8316), c.e(7066), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(7505), c.e(1514), c.e(7968), c.e(8930), c.e(5238), c.e(5320)]).then((() => () => c(97066))))), i("@jupyterlab/apputils", "3.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(8316), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(988), c.e(7505), c.e(8695), c.e(1514), c.e(4812), c.e(8930), c.e(1732)]).then((() => () => c(90339))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(286), c.e(4947), c.e(2233), c.e(6616)]).then((() => () => c(20286))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(2233), c.e(709)]).then((() => () => c(62359))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(2233), c.e(6178)]).then((() => () => c(70053))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(3922), c.e(4947), c.e(2233), c.e(2630)]).then((() => () => c(13922))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(2233), c.e(6614)]).then((() => () => c(20596))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(2233), c.e(1023)]).then((() => () => c(1980))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(2233), c.e(6790)]).then((() => () => c(4896))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(2233), c.e(3086)]).then((() => () => c(60103))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(2950), c.e(4947), c.e(2233), c.e(1667)]).then((() => () => c(42950))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(3251), c.e(4947), c.e(2233), c.e(7623)]).then((() => () => c(53251))))), i("@jupyterlab/docregistry", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(2299), c.e(7505), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))), i("@jupyterlab/json-extension", "3.6.3", (() => Promise.all([c.e(8316), c.e(5950), c.e(2233), c.e(6956), c.e(2051), c.e(7782), c.e(4643), c.e(7505)]).then((() => () => c(45950))))), i("@jupyterlab/logconsole", "3.6.3", (() => Promise.all([c.e(9339), c.e(4947), c.e(2233), c.e(6956), c.e(2051), c.e(2299), c.e(3198)]).then((() => () => c(99339))))), i("@jupyterlab/mainmenu", "3.6.3", (() => Promise.all([c.e(2233), c.e(3203), c.e(2051), c.e(4643), c.e(1581)]).then((() => () => c(21581))))), i("@jupyterlab/markdownviewer-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(2299), c.e(7968), c.e(8930), c.e(5238), c.e(4382)]).then((() => () => c(54382))))), i("@jupyterlab/mathjax2-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(9110), c.e(2299), c.e(6976)]).then((() => () => c(66976))))), i("@jupyterlab/nbformat", "3.6.3", (() => Promise.all([c.e(2233), c.e(3655)]).then((() => () => c(63655))))), i("@jupyterlab/notebook", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(7505), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(3198), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))), i("@jupyterlab/outputarea", "3.6.3", (() => Promise.all([c.e(1432), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(4629), c.e(7782), c.e(988), c.e(2299), c.e(9939)]).then((() => () => c(31432))))), i("@jupyterlab/rendermime-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(7782), c.e(2299), c.e(5985)]).then((() => () => c(85985))))), i("@jupyterlab/rendermime", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(846), c.e(7560), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9098), c.e(3008)]).then((() => () => c(17560))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(74), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9320)]).then((() => () => c(80074))))), i("@jupyterlab/services", "6.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9110), c.e(1497)]).then((() => () => c(16914))))), i("@jupyterlab/settingregistry", "3.6.3", (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(2233), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))), i("@jupyterlab/theme-dark-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(1058)]).then((() => () => c(21058))))), i("@jupyterlab/theme-light-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(275)]).then((() => () => c(60275))))), i("@jupyterlab/translation", "3.6.3", (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))), i("@jupyterlab/ui-components", "3.6.3", (() => Promise.all([c.e(6770), c.e(8316), c.e(4963), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7505), c.e(2886)]).then((() => () => c(74963))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([c.e(9757), c.e(2233), c.e(9110)]).then((() => () => c(9757))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([c.e(2233), c.e(2051), c.e(6527)]).then((() => () => c(26527))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(2233), c.e(5820)]).then((() => () => c(83693))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([c.e(6111), c.e(4530), c.e(2233), c.e(3203), c.e(4456), c.e(7631), c.e(3862)]).then((() => () => c(24530))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2233), c.e(2051), c.e(1514), c.e(568), c.e(3256)]).then((() => () => c(93256))))), i("@lumino/algorithm", "1.9.2", (() => c.e(9060).then((() => () => c(69060))))), i("@lumino/algorithm", "2.0.0", (() => c.e(9807).then((() => () => c(89807))))), i("@lumino/commands", "1.21.1", (() => Promise.all([c.e(2687), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))), i("@lumino/coreutils", "1.12.1", (() => c.e(1770).then((() => () => c(71770))))), i("@lumino/coreutils", "2.1.0", (() => c.e(4259).then((() => () => c(4259))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))), i("@lumino/domutils", "1.8.2", (() => c.e(5403).then((() => () => c(85403))))), i("@lumino/dragdrop", "1.14.5", (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))), i("@lumino/properties", "1.8.2", (() => c.e(3312).then((() => () => c(73312))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))), i("@lumino/signaling", "2.1.0", (() => Promise.all([c.e(6088), c.e(319), c.e(7003)]).then((() => () => c(27003))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([c.e(1053), c.e(3203)]).then((() => () => c(1053))))), i("@lumino/widgets", "1.37.2", (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))), i("@voila-dashboards/voila", "0.5.0-alpha.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(988), c.e(2299), c.e(7651), c.e(5238), c.e(5918), c.e(3504)]).then((() => () => c(17696))))), i("react", "17.0.2", (() => c.e(2784).then((() => () => c(2784)))))), e[l] = u.length ? Promise.all(u).then((() => e[l] = 1)) : 1
+                return "default" === l && (i("@jupyter-widgets/base", "6.0.4", (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))), i("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([c.e(8291), c.e(3851), c.e(4947), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(7651), c.e(6587)]).then((() => () => c(53851))))), i("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(988), c.e(2299), c.e(8930), c.e(3198), c.e(7651), c.e(49), c.e(5320), c.e(6678), c.e(2266)]).then((() => () => c(9727))))), i("@jupyter-widgets/output", "6.0.4", (() => Promise.all([c.e(7651), c.e(1100)]).then((() => () => c(21100))))), i("@jupyterlab/application", "3.6.3", (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))), i("@jupyterlab/apputils-extension", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5238), c.e(5320)]).then((() => () => c(97066))))), i("@jupyterlab/apputils", "3.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(1514), c.e(4812), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(286), c.e(4947), c.e(2233), c.e(6616)]).then((() => () => c(20286))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(2233), c.e(709)]).then((() => () => c(62359))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(2233), c.e(6178)]).then((() => () => c(70053))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(3922), c.e(4947), c.e(2233), c.e(2630)]).then((() => () => c(13922))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(2233), c.e(6614)]).then((() => () => c(20596))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(2233), c.e(1023)]).then((() => () => c(1980))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(2233), c.e(6790)]).then((() => () => c(4896))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(2233), c.e(3086)]).then((() => () => c(60103))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(2950), c.e(4947), c.e(2233), c.e(1667)]).then((() => () => c(42950))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(3251), c.e(4947), c.e(2233), c.e(7623)]).then((() => () => c(53251))))), i("@jupyterlab/docregistry", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(2299), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))), i("@jupyterlab/json-extension", "3.6.3", (() => Promise.all([c.e(5950), c.e(2233), c.e(6956), c.e(2051), c.e(7782), c.e(4643), c.e(7505), c.e(4627)]).then((() => () => c(45950))))), i("@jupyterlab/logconsole", "3.6.3", (() => Promise.all([c.e(9339), c.e(4947), c.e(2233), c.e(6956), c.e(2051), c.e(2299), c.e(3198)]).then((() => () => c(99339))))), i("@jupyterlab/mainmenu", "3.6.3", (() => Promise.all([c.e(2233), c.e(3203), c.e(2051), c.e(4643), c.e(1581)]).then((() => () => c(21581))))), i("@jupyterlab/markdownviewer-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(2299), c.e(7968), c.e(8930), c.e(5238), c.e(4382)]).then((() => () => c(54382))))), i("@jupyterlab/mathjax2-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(9110), c.e(2299), c.e(6976)]).then((() => () => c(66976))))), i("@jupyterlab/nbformat", "3.6.3", (() => Promise.all([c.e(2233), c.e(3655)]).then((() => () => c(63655))))), i("@jupyterlab/notebook", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(2299), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(3198), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))), i("@jupyterlab/outputarea", "3.6.3", (() => Promise.all([c.e(1432), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(4629), c.e(7782), c.e(988), c.e(2299), c.e(9939)]).then((() => () => c(31432))))), i("@jupyterlab/rendermime-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(7782), c.e(2299), c.e(5985)]).then((() => () => c(85985))))), i("@jupyterlab/rendermime", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(846), c.e(7560), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9098), c.e(3008)]).then((() => () => c(17560))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(74), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9320)]).then((() => () => c(80074))))), i("@jupyterlab/services", "6.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9110), c.e(1497)]).then((() => () => c(16914))))), i("@jupyterlab/settingregistry", "3.6.3", (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(2233), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))), i("@jupyterlab/theme-dark-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(1058)]).then((() => () => c(21058))))), i("@jupyterlab/theme-light-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(275)]).then((() => () => c(60275))))), i("@jupyterlab/translation", "3.6.3", (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))), i("@jupyterlab/ui-components", "3.6.3", (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([c.e(9757), c.e(2233), c.e(9110)]).then((() => () => c(9757))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([c.e(2233), c.e(2051), c.e(6527)]).then((() => () => c(26527))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(2233), c.e(5820)]).then((() => () => c(83693))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([c.e(6111), c.e(4530), c.e(2233), c.e(3203), c.e(4456), c.e(7631), c.e(3862)]).then((() => () => c(24530))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2233), c.e(2051), c.e(1514), c.e(568), c.e(3256)]).then((() => () => c(93256))))), i("@lumino/algorithm", "1.9.2", (() => c.e(9060).then((() => () => c(69060))))), i("@lumino/algorithm", "2.0.0", (() => c.e(9807).then((() => () => c(89807))))), i("@lumino/commands", "1.21.1", (() => Promise.all([c.e(2687), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))), i("@lumino/coreutils", "1.12.1", (() => c.e(1770).then((() => () => c(71770))))), i("@lumino/coreutils", "2.1.0", (() => c.e(4259).then((() => () => c(4259))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))), i("@lumino/domutils", "1.8.2", (() => c.e(5403).then((() => () => c(85403))))), i("@lumino/dragdrop", "1.14.5", (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))), i("@lumino/properties", "1.8.2", (() => c.e(3312).then((() => () => c(73312))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))), i("@lumino/signaling", "2.1.0", (() => Promise.all([c.e(6088), c.e(319), c.e(7003)]).then((() => () => c(27003))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([c.e(1053), c.e(3203)]).then((() => () => c(1053))))), i("@lumino/widgets", "1.37.2", (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))), i("@voila-dashboards/voila", "0.5.0-alpha.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(988), c.e(2299), c.e(7651), c.e(5238), c.e(5918), c.e(3504)]).then((() => () => c(17696))))), i("react-dom", "17.0.2", (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))), i("react", "17.0.2", (() => c.e(2784).then((() => () => c(2784)))))), e[l] = u.length ? Promise.all(u).then((() => e[l] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         c.g.importScripts && (e = c.g.location + "");
         var t = c.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
@@ -144,88 +144,89 @@
     }, o = (e, t) => {
         if (0 in e) {
             t = a(t);
             var l = e[0],
                 r = l < 0;
             r && (l = -l - 1);
             for (var n = 0, i = 1, u = !0;; i++, n++) {
-                var s, m, p = i < e.length ? (typeof e[i])[0] : "";
-                if (n >= t.length || "o" == (m = (typeof(s = t[n]))[0])) return !u || ("u" == p ? i > l && !r : "" == p != r);
+                var s, m, h = i < e.length ? (typeof e[i])[0] : "";
+                if (n >= t.length || "o" == (m = (typeof(s = t[n]))[0])) return !u || ("u" == h ? i > l && !r : "" == h != r);
                 if ("u" == m) {
-                    if (!u || "u" != p) return !1
+                    if (!u || "u" != h) return !1
                 } else if (u)
-                    if (p == m)
+                    if (h == m)
                         if (i <= l) {
                             if (s != e[i]) return !1
                         } else {
                             if (r ? s > e[i] : s < e[i]) return !1;
                             s != e[i] && (u = !1)
                         }
-                else if ("s" != p && "n" != p) {
+                else if ("s" != h && "n" != h) {
                     if (r || i <= l) return !1;
                     u = !1, i--
                 } else {
-                    if (i <= l || m < p != r) return !1;
+                    if (i <= l || m < h != r) return !1;
                     u = !1
-                } else "s" != p && "n" != p && (u = !1, i--)
+                } else "s" != h && "n" != h && (u = !1, i--)
             }
         }
-        var h = [],
-            d = h.pop.bind(h);
+        var p = [],
+            d = p.pop.bind(p);
         for (n = 1; n < e.length; n++) {
             var f = e[n];
-            h.push(1 == f ? d() | d() : 2 == f ? d() & d() : f ? o(f, t) : !d())
+            p.push(1 == f ? d() | d() : 2 == f ? d() & d() : f ? o(f, t) : !d())
         }
         return !!d()
     }, i = (e, t, l) => {
         var r = e[t];
         return (t = Object.keys(r).reduce(((e, t) => !o(l, t) || e && !n(e, t) ? e : t), 0)) && r[t]
     }, u = e => (e.loaded = 1, e.get()), s = (e => function(t, l, r, a) {
         var n = c.I(t);
         return n && n.then ? n.then(e.bind(e, t, c.S[t], l, r, a)) : e(0, c.S[t], l, r, a)
     })(((e, t, l, r, a) => {
         var n = t && c.o(t, l) && i(t, l, r);
         return n ? u(n) : a()
-    })), m = {}, p = {
+    })), m = {}, h = {
         92233: () => s("default", "@lumino/coreutils", [1, 1, 8, 2], (() => c.e(1770).then((() => () => c(71770))))),
         42051: () => s("default", "@lumino/widgets", [1, 1, 26, 2], (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))),
         59110: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(6196)]).then((() => () => c(60103))))),
-        37782: () => s("default", "@jupyterlab/apputils", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(846), c.e(8316), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(988), c.e(7505), c.e(8695), c.e(1514), c.e(4812), c.e(8930), c.e(1732)]).then((() => () => c(90339))))),
+        37782: () => s("default", "@jupyterlab/apputils", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(1514), c.e(4812), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))),
         12299: () => s("default", "@jupyterlab/rendermime", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))),
+        24627: () => s("default", "react-dom", [1, 17, 0, 1], (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))),
         73198: () => s("default", "@jupyterlab/outputarea", [1, 3, 0, 0], (() => Promise.all([c.e(1432), c.e(4947), c.e(3203), c.e(4629), c.e(7782), c.e(988), c.e(9939)]).then((() => () => c(31432))))),
         67651: () => s("default", "@jupyter-widgets/base", [1, 6, 0, 1], (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))),
         75238: () => s("default", "@jupyterlab/application", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))),
-        40049: () => s("default", "@jupyterlab/notebook", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(7505), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))),
+        40049: () => s("default", "@jupyterlab/notebook", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))),
         94456: () => s("default", "@jupyterlite/server", [2, 0, 1, 0], (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2051), c.e(1514), c.e(568), c.e(6856)]).then((() => () => c(93256))))),
         7631: () => s("default", "@jupyterlite/kernel", [2, 0, 1, 0], (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(5820)]).then((() => () => c(83693))))),
         35918: () => s("default", "@jupyter-widgets/jupyterlab-manager", [1, 5, 0, 3], (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(988), c.e(8930), c.e(3198), c.e(49), c.e(5320), c.e(6678), c.e(2516)]).then((() => () => c(9727))))),
-        9961: () => s("default", "@jupyterlab/apputils-extension", [1, 3, 4, 8], (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(8316), c.e(7066), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(4643), c.e(988), c.e(7505), c.e(1514), c.e(7968), c.e(8930), c.e(5320)]).then((() => () => c(97066))))),
+        9961: () => s("default", "@jupyterlab/apputils-extension", [1, 3, 4, 8], (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5320)]).then((() => () => c(97066))))),
         22312: () => s("default", "@voila-dashboards/voila", [2, 0, 5, 0, , "alpha", 3], (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(988), c.e(2230)]).then((() => () => c(17696))))),
         59601: () => s("default", "@jupyterlab/theme-dark-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6956), c.e(3811)]).then((() => () => c(21058))))),
         99661: () => s("default", "@jupyterlab/theme-light-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6956), c.e(7469)]).then((() => () => c(60275))))),
         4319: () => s("default", "@jupyterlab/markdownviewer-extension", [1, 3, 0, 0], (() => Promise.all([c.e(6956), c.e(7968), c.e(8930), c.e(6757)]).then((() => () => c(54382))))),
         24132: () => s("default", "@jupyterlab/mathjax2-extension", [1, 3, 0, 0], (() => c.e(3349).then((() => () => c(66976))))),
         41412: () => s("default", "@jupyterlab/rendermime-extension", [1, 3, 0, 0], (() => Promise.all([c.e(6956), c.e(3305)]).then((() => () => c(85985))))),
-        70851: () => s("default", "@jupyterlab/json-extension", [1, 3, 0, 0], (() => Promise.all([c.e(8316), c.e(5950), c.e(6956), c.e(4643), c.e(7505)]).then((() => () => c(45950))))),
+        70851: () => s("default", "@jupyterlab/json-extension", [1, 3, 0, 0], (() => Promise.all([c.e(5950), c.e(6956), c.e(4643), c.e(7505)]).then((() => () => c(45950))))),
         84632: () => s("default", "@jupyterlite/iframe-extension", [2, 0, 1, 0], (() => c.e(5826).then((() => () => c(26527))))),
         78695: () => s("default", "@lumino/messaging", [1, 1, 7, 2], (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))),
         4947: () => s("default", "@lumino/signaling", [1, 1, 7, 2], (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))),
         23203: () => s("default", "@lumino/algorithm", [1, 1, 6, 2], (() => c.e(9060).then((() => () => c(69060))))),
         94812: () => s("default", "@lumino/domutils", [1, 1, 5, 2], (() => c.e(5403).then((() => () => c(85403))))),
         36e3: () => s("default", "@lumino/disposable", [1, 1, 7, 2], (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))),
         56956: () => s("default", "@jupyterlab/translation", [1, 3, 0, 0], (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))),
         24629: () => s("default", "@lumino/properties", [1, 1, 5, 2], (() => c.e(3312).then((() => () => c(73312))))),
         70988: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(3203), c.e(6e3), c.e(9110), c.e(6417)]).then((() => () => c(16914))))),
         68930: () => s("default", "@jupyterlab/settingregistry", [1, 3, 0, 0], (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))),
         5320: () => s("default", "@jupyterlab/mainmenu", [1, 3, 0, 0], (() => Promise.all([c.e(4643), c.e(9406)]).then((() => () => c(21581))))),
         10409: () => s("default", "@jupyter-widgets/output", [1, 6, 0, 1], (() => c.e(7015).then((() => () => c(21100))))),
         70190: () => s("default", "@jupyterlab/logconsole", [1, 3, 0, 0], (() => c.e(9339).then((() => () => c(99339))))),
-        24643: () => s("default", "@jupyterlab/ui-components", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(8316), c.e(4963), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(9110), c.e(7505), c.e(2886)]).then((() => () => c(74963))))),
+        24643: () => s("default", "@jupyterlab/ui-components", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))),
         1514: () => s("default", "@lumino/commands", [1, 1, 15, 2], (() => Promise.all([c.e(2687), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))),
-        77968: () => s("default", "@jupyterlab/docregistry", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(3203), c.e(6e3), c.e(4643), c.e(2299), c.e(7505), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))),
+        77968: () => s("default", "@jupyterlab/docregistry", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(3203), c.e(6e3), c.e(4643), c.e(7505), c.e(2299), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))),
         97505: () => s("default", "react", [1, 17, 0, 1], (() => c.e(2784).then((() => () => c(2784))))),
         56088: () => s("default", "@lumino/coreutils", [1, 1, 8, 2], (() => c.e(4259).then((() => () => c(4259))))),
         91876: () => s("default", "@lumino/signaling", [1, 1, 7, 2], (() => Promise.all([c.e(319), c.e(1553)]).then((() => () => c(27003))))),
         49939: () => s("default", "@jupyterlab/nbformat", [1, 3, 0, 0], (() => c.e(86).then((() => () => c(63655))))),
         32886: () => s("default", "@lumino/virtualdom", [1, 1, 11, 2], (() => c.e(1053).then((() => () => c(1053))))),
         3860: () => s("default", "@lumino/dragdrop", [1, 1, 10, 2], (() => c.e(8809).then((() => () => c(38809))))),
         89098: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(2950), c.e(1105)]).then((() => () => c(42950))))),
@@ -239,15 +240,15 @@
         81298: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(7795)]).then((() => () => c(20596))))),
         91491: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(5291)]).then((() => () => c(4896))))),
         2132: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(74), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9817)]).then((() => () => c(80074))))),
         86086: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(3922), c.e(8874)]).then((() => () => c(13922))))),
         90319: () => s("default", "@lumino/algorithm", [1, 1, 6, 2], (() => c.e(9807).then((() => () => c(89807))))),
         7531: () => s("default", "@jupyterlite/server-extension", [2, 0, 1, 0], (() => Promise.all([c.e(6111), c.e(4530), c.e(3203), c.e(7631), c.e(3862)]).then((() => () => c(24530))))),
         17021: () => s("default", "@jupyter-widgets/controls", [1, 5, 0, 1], (() => Promise.all([c.e(3851), c.e(8695), c.e(4812)]).then((() => () => c(53851)))))
-    }, h = {
+    }, p = {
         49: [40049],
         319: [90319],
         568: [2132, 86086],
         988: [70988],
         1514: [1514],
         1876: [91876],
         2051: [42051],
@@ -255,14 +256,15 @@
         2299: [12299],
         2886: [32886],
         3198: [73198],
         3203: [23203],
         3860: [3860],
         3862: [48753, 52329, 52390, 70771, 81298, 91491],
         4456: [94456],
+        4627: [24627],
         4629: [24629],
         4643: [24643],
         4812: [94812],
         4863: [17021],
         4947: [4947],
         5238: [75238],
         5320: [5320],
@@ -283,42 +285,42 @@
         8695: [78695],
         8930: [68930],
         8987: [9961, 22312, 59601, 99661],
         9098: [89098],
         9110: [59110],
         9939: [49939]
     }, c.f.consumes = (e, t) => {
-        c.o(h, e) && h[e].forEach((e => {
+        c.o(p, e) && p[e].forEach((e => {
             if (c.o(m, e)) return t.push(m[e]);
             var l = t => {
                     m[e] = 0, c.m[e] = l => {
                         delete c.c[e], l.exports = t()
                     }
                 },
                 r = t => {
                     delete m[e], c.m[e] = l => {
                         throw delete c.c[e], t
                     }
                 };
             try {
-                var a = p[e]();
+                var a = h[e]();
                 a.then ? t.push(m[e] = a.then(l).catch(r)) : l(a)
             } catch (e) {
                 r(e)
             }
         }))
     }, (() => {
         var e = {
             6684: 0
         };
         c.f.j = (t, l) => {
             var r = c.o(e, t) ? e[t] : void 0;
             if (0 !== r)
                 if (r) l.push(r[2]);
-                else if (/^(2(051|233|299|886)|3(19(|8)|86[02]|203)|4(456|629|643|812|863|9|947)|5((23|6|91)8|(32|49|82)0)|6(000|088|678|956)|7((53|63|65)1|505|782|968)|8(695|930|987)|9(098|110|88|939)|1514|1876)$/.test(t)) e[t] = 0;
+                else if (/^(2(051|233|299|886)|3(19(|8)|86[02]|203)|4(6(27|29|43)|456|812|863|9|947)|5((23|6|91)8|(32|49|82)0)|6(000|088|678|956)|7((53|63|65)1|505|782|968)|8(695|930|987)|9(098|110|88|939)|1514|1876)$/.test(t)) e[t] = 0;
             else {
                 var a = new Promise(((l, a) => r = e[t] = [l, a]));
                 l.push(r[2] = a);
                 var n = c.p + c.u(t),
                     o = new Error;
                 c.l(n, (l => {
                     if (c.o(e, t) && (0 !== (r = e[t]) && (e[t] = void 0), r)) {
```

### Comparing `voici-0.4.0/LICENSE` & `voici-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/README.md` & `voici-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/pyproject.toml` & `voici-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `voici-0.4.0/PKG-INFO` & `voici-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voici
-Version: 0.4.0
+Version: 0.4.1
 Summary: Voici turns Jupyter notebooks into static web applications
 Project-URL: Homepage, https://github.com/voila-dashboards/voici
 Author: Voila Development Team
 License: BSD License
         
         Copyright (c) 2018 Voilà contributors.
         All rights reserved.
```

