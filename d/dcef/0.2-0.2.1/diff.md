# Comparing `tmp/dcef-0.2.tar.gz` & `tmp/dcef-0.2.1.tar.gz`

## Comparing `dcef-0.2.tar` & `dcef-0.2.1.tar`

### file list

```diff
@@ -1,78 +1,104 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dcef-0.2/.coveragerc
--rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 dcef-0.2/ENV.txt
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 dcef-0.2/RELEASE.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dcef-0.2/babel.config.js
--rwxr-xr-x   0        0        0      232 2020-02-02 00:00:00.000000 dcef-0.2/full_build.sh
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 dcef-0.2/introduction.ipynb
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid.json
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 dcef-0.2/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dcef-0.2/setup.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 dcef-0.2/tryit.ipynb
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dcef-0.2/tsconfig.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcef-0.2/video_script.txt
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dcef-0.2/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 dcef-0.2/webpack.lab.config.js
--rw-r--r--   0        0        0   401763 2020-02-02 00:00:00.000000 dcef-0.2/yarn.lock
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dcef-0.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 dcef-0.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dcef-0.2/.pytest_cache/README.md
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 dcef-0.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcef-0.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dcef-0.2/dcf/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 dcef-0.2/dcf/_frontend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dcef-0.2/dcf/_version.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 dcef-0.2/dcf/all_transforms.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 dcef-0.2/dcf/channeldata.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 dcef-0.2/dcf/configure_utils.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 dcef-0.2/dcf/dcf_transform.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 dcef-0.2/dcf/dcf_widget.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dcef-0.2/dcf/df_methods.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 dcef-0.2/dcf/index.html
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 dcef-0.2/dcf/lispy.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 dcef-0.2/dcf/views.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2/dcf/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2/dcf/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 dcef-0.2/dcf/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2/dcf/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2/dcf/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2/dcf/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2/dcf/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dcef-0.2/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/_frontend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/_version.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/paddy_widget.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/package.json
--rw-r--r--   0        0        0  1235644 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/116.e2ccbe733d0a9edd1777.js
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/116.e2ccbe733d0a9edd1777.js.LICENSE.txt
--rw-r--r--   0        0        0   372521 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/250.970b486f665683a12362.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/250.970b486f665683a12362.js.LICENSE.txt
--rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/480.a1fc9bd0ae29c3af7210.js
--rw-r--r--   0        0        0    70509 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/486.3a86dcecb5e722e84edc.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/486.3a86dcecb5e722e84edc.js.LICENSE.txt
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/568.c9e5ec7d47bb9db3ae77.js
--rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/remoteEntry.8a6d805ad1f7bc974c84.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/style.js
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0  1690452 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/nbextension/index.js
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0  5597377 2020-02-02 00:00:00.000000 dcef-0.2/ipydatagrid/nbextension/index.js.map
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 dcef-0.2/js/dcfwidget.ts
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 dcef-0.2/js/extension.ts
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dcef-0.2/js/index.ts
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 dcef-0.2/js/paddywidget.ts
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 dcef-0.2/js/plugin.ts
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 dcef-0.2/js/version.ts
--rw-r--r--   0        0        0  1099577 2020-02-02 00:00:00.000000 dcef-0.2/static/images/Dcf-tabbed.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dcef-0.2/style/widget.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dcef-0.2/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 dcef-0.2/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dcef-0.2/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 dcef-0.2/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 dcef-0.2/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 dcef-0.2/style/icons/filter.svg
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 dcef-0.2/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 dcef-0.2/LICENSE.txt
--rw-r--r--   0        0        0    12508 2020-02-02 00:00:00.000000 dcef-0.2/README.md
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 dcef-0.2/pyproject.toml
--rw-r--r--   0        0        0    15312 2020-02-02 00:00:00.000000 dcef-0.2/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.1/.#video_script.txt -> paddy@Paddys-Air.routerlogin.net.2877
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dcef-0.2.1/.coveragerc
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 dcef-0.2.1/ENV.txt
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 dcef-0.2.1/RELEASE.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dcef-0.2.1/babel.config.js
+-rwxr-xr-x   0        0        0      232 2020-02-02 00:00:00.000000 dcef-0.2.1/full_build.sh
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 dcef-0.2.1/introduction.ipynb
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid.json
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 dcef-0.2.1/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dcef-0.2.1/setup.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 dcef-0.2.1/tryit.ipynb
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dcef-0.2.1/tsconfig.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcef-0.2.1/video_script.txt
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dcef-0.2.1/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 dcef-0.2.1/webpack.lab.config.js
+-rw-r--r--   0        0        0   401763 2020-02-02 00:00:00.000000 dcef-0.2.1/yarn.lock
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dcef-0.2.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 dcef-0.2.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dcef-0.2.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 dcef-0.2.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcef-0.2.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/_frontend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/_version.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/all_transforms.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/channeldata.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/configure_utils.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/dcef_widget.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/dcf_transform.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/df_methods.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/index.html
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/lispy.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/views.py
+-rw-r--r--   0        0        0    20309 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/build_log.json
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/package.json
+-rw-r--r--   0        0        0    13801 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/lib_index_js.4cd4476fba62a32f32e7.js
+-rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/lib_index_js.4cd4476fba62a32f32e7.js.map
+-rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/lib_plugin_js.0eece56301a1622da4db.js
+-rw-r--r--   0        0        0    11564 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/lib_plugin_js.0eece56301a1622da4db.js.map
+-rw-r--r--   0        0        0    30708 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/remoteEntry.42e89f8f6eba485d64ec.js
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/remoteEntry.42e89f8f6eba485d64ec.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/style.js
+-rw-r--r--   0        0        0  1144785 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_react-dom_index_js-node_modu-da96ce.362c78a0fe737b7728ed.js
+-rw-r--r--   0        0        0  1338317 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_react-dom_index_js-node_modu-da96ce.362c78a0fe737b7728ed.js.map
+-rw-r--r--   0        0        0   544593 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/vendors-node_modules_lodash_lodash_js.72dd6d901a8f2c6586e9.js
+-rw-r--r--   0        0        0   670363 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/vendors-node_modules_lodash_lodash_js.72dd6d901a8f2c6586e9.js.map
+-rw-r--r--   0        0        0   232796 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/vendors-node_modules_paddy-react-edit-list_index_js.1e88d9d01d30d2904ab5.js
+-rw-r--r--   0        0        0   380329 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/labextension/static/vendors-node_modules_paddy-react-edit-list_index_js.1e88d9d01d30d2904ab5.js.map
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/nbextension/extension.js
+-rw-r--r--   0        0        0   309093 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/nbextension/index.js
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  1359025 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/nbextension/index.js.map
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.1/dcef/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dcef-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 dcef-0.2.1/docs/commands_vs_operations.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcef-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 dcef-0.2.1/docs/source/FAQ.rst
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 dcef-0.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 dcef-0.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dcef-0.2.1/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/_frontend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/_version.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/paddy_widget.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/package.json
+-rw-r--r--   0        0        0  1235644 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/116.e2ccbe733d0a9edd1777.js
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/116.e2ccbe733d0a9edd1777.js.LICENSE.txt
+-rw-r--r--   0        0        0   372521 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/250.970b486f665683a12362.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/250.970b486f665683a12362.js.LICENSE.txt
+-rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/480.a1fc9bd0ae29c3af7210.js
+-rw-r--r--   0        0        0    70509 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/486.3a86dcecb5e722e84edc.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/486.3a86dcecb5e722e84edc.js.LICENSE.txt
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/568.c9e5ec7d47bb9db3ae77.js
+-rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/remoteEntry.7f7af2d8c54c49567ac4.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/style.js
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0  1690452 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/nbextension/index.js
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  5597377 2020-02-02 00:00:00.000000 dcef-0.2.1/ipydatagrid/nbextension/index.js.map
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 dcef-0.2.1/js/dcfwidget.ts
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 dcef-0.2.1/js/extension.ts
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dcef-0.2.1/js/index.ts
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 dcef-0.2.1/js/paddywidget.ts
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 dcef-0.2.1/js/plugin.ts
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 dcef-0.2.1/js/version.ts
+-rw-r--r--   0        0        0  1335815 2020-02-02 00:00:00.000000 dcef-0.2.1/static/images/dcf-jupyter.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dcef-0.2.1/style/widget.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dcef-0.2.1/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 dcef-0.2.1/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dcef-0.2.1/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 dcef-0.2.1/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 dcef-0.2.1/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 dcef-0.2.1/style/icons/filter.svg
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 dcef-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 dcef-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 dcef-0.2.1/README.md
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 dcef-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12656 2020-02-02 00:00:00.000000 dcef-0.2.1/PKG-INFO
```

### Comparing `dcef-0.2/ENV.txt` & `dcef-0.2.1/ENV.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2/RELEASE.md` & `dcef-0.2.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `dcef-0.2/introduction.ipynb` & `dcef-0.2.1/tryit.ipynb`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9324652777777778%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import json\\n'), (2, 'import numpy as np\\n')]}}, 1: "*

 * *            '{\'source\': {insert: [(1, "df2 = '*

 * *            'pd.read_csv(\'./examples/data/yellow_tripdata_2021-02.csv\')")], delete: [2, 1]}}, 2: '*

 * *            "{'source': ['w = DCFWidget(df=df2)\\n', 'w']}, 3: {'source': ['transformed_df = "*

 * *            'w.dcf_transform(w.commands, w.df)\\n\', "w.transformed_df = '*

 * *            'json.loads(transformed_df.to_json(orient=\'table\', indent=2))"]}, 4: {\'source\ […]*

```diff
@@ -3,120 +3,56 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
+                "import json\n",
+                "import numpy as np\n",
                 "from dcf.dcf_widget import DCFWidget"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = pd.read_csv('./examples/data/2014-01-citibike-tripdata.csv')\n",
-                "w = DCFWidget(df)\n",
-                "w"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from dcf.all_transforms import Transform\n",
-                "from dcf.lispy import s\n",
-                "#Here we start adding commands to the DCF Widget.  Every call to add_command replaces a command with the same name\n",
-                "@w.add_command\n",
-                "class GroupBy2(Transform):\n",
-                "    command_default = [s(\"groupby2\"), s('df'), 'col', {}]\n",
-                "    command_pattern = [[3, 'colMap', 'colEnum', ['null', 'sum', 'mean', 'median', 'count']]]\n",
-                "    @staticmethod \n",
-                "    def transform(df, col, col_spec):\n",
-                "        grps = df.groupby(col)\n",
-                "        df_contents = {}\n",
-                "        for k, v in col_spec.items():\n",
-                "            if v == \"sum\":\n",
-                "                df_contents[k] = grps[k].apply(lambda x: x.sum())\n",
-                "            elif v == \"mean\":\n",
-                "                df_contents[k] = grps[k].apply(lambda x: x.mean())\n",
-                "            elif v == \"median\":\n",
-                "                df_contents[k] = grps[k].apply(lambda x: x.median())\n",
-                "            elif v == \"count\":\n",
-                "                df_contents[k] = grps[k].apply(lambda x: x.count())\n",
-                "        return pd.DataFrame(df_contents)\n",
-                "\n",
-                "    @staticmethod \n",
-                "    def transform_to_py(df, col, col_spec):\n",
-                "        commands = [\n",
-                "            \"    grps = df.groupby('%s')\" % col,\n",
-                "            \"    df_contents = {}\"\n",
-                "        ]\n",
-                "        for k, v in col_spec.items():\n",
-                "            if v == \"sum\":\n",
-                "                commands.append(\"    paddydf_contents['%s'] = grps['%s'].apply(lambda x: x.sum())\" % (k, k))\n",
-                "            elif v == \"mean\":\n",
-                "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.mean())\" % (k, k))\n",
-                "            elif v == \"median\":\n",
-                "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.median())\" % (k, k))\n",
-                "            elif v == \"count\":\n",
-                "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.count())\" % (k, k))\n",
-                "        commands.append(\"    df = pd.DataFrame(df_contents)\")\n",
-                "        return \"\\n\".join(commands)\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "w.operation_results = {\n",
-                "    'transformed_df':w.js_df,\n",
-                "    'generated_py_code':'#from py widget init'}"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "bc = [{'symbol': 'begin'}, [{'symbol': 'dropcol'}, {'symbol': 'df'}, 'stoptime']]"
+                "df2 = pd.read_csv('./examples/data/yellow_tripdata_2021-02.csv')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "w.commands = bc"
+                "w = DCFWidget(df=df2)\n",
+                "w"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "w.operation_results['generated_py_code']"
+                "transformed_df = w.dcf_transform(w.commands, w.df)\n",
+                "w.transformed_df = json.loads(transformed_df.to_json(orient='table', indent=2))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(dict(foo=3,bar=5).keys())"
+                "w.commands"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -126,88 +62,77 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "w.generated_py_code = \"paddy\""
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "w.commands = [bc[0]]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ab = [{'symbol': 'begin'},\n",
-                " [{'symbol': 'dropcol'}, {'symbol': 'df'}, 'stoptime'],\n",
-                " [{'symbol': 'onehot'}, {'symbol': 'df'}, 'stoptime']]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "w.command_config = w.command_config"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "transformed_df = w.dcf_transform(w.commands, w.df)\n",
-                "w.transformed_df = json.loads(transformed_df.to_json(orient='table', indent=2))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "w.commands"
+                "w.generated_py_code = w.dcf_to_py_core(w.commands[1:])\n",
+                "w.generated_py_code"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(w.generated_py_code)"
+                "from dcf.all_transforms import Transform\n",
+                "from dcf.lispy import s"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
             "source": [
-                "df2 = pd.read_csv('./examples/data/yellow_tripdata_2021-02.csv')"
+                "@w.add_command\n",
+                "class GroupBy2(Transform):\n",
+                "    command_default = [s(\"groupby2\"), s('df'), 'col', {}]\n",
+                "    command_pattern = [[3, 'colMap', 'colEnum', ['null', 'sum', 'mean', 'median', 'count']]]\n",
+                "    @staticmethod \n",
+                "    def transform(df, col, col_spec):\n",
+                "        grps = df.groupby(col)\n",
+                "        df_contents = {}\n",
+                "        for k, v in col_spec.items():\n",
+                "            if v == \"sum\":\n",
+                "                df_contents[k] = grps[k].apply(lambda x: x.sum())\n",
+                "            elif v == \"mean\":\n",
+                "                df_contents[k] = grps[k].apply(lambda x: x.mean())\n",
+                "            elif v == \"median\":\n",
+                "                df_contents[k] = grps[k].apply(lambda x: x.median())\n",
+                "            elif v == \"count\":\n",
+                "                df_contents[k] = grps[k].apply(lambda x: x.count())\n",
+                "        return pd.DataFrame(df_contents)\n",
+                "\n",
+                "    #test_df = group_df\n",
+                "    #test_sequence = [s(\"groupby2\"), s('df'), 'c', dict(a='sum', b='mean')]\n",
+                "    test_output = pd.DataFrame(\n",
+                "        {'a':[100, 110], 'b':[2.5, 5.5]},\n",
+                "        index=['q','w'])\n",
+                "\n",
+                "    @staticmethod \n",
+                "    def transform_to_py(df, col, col_spec):\n",
+                "        commands = [\n",
+                "            \"    grps = df.groupby('%s')\" % col,\n",
+                "            \"    df_contents = {}\"\n",
+                "        ]\n",
+                "        for k, v in col_spec.items():\n",
+                "            if v == \"sum\":\n",
+                "                commands.append(\"    paddydf_contents['%s'] = grps['%s'].apply(lambda x: x.sum())\" % (k, k))\n",
+                "            elif v == \"mean\":\n",
+                "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.mean())\" % (k, k))\n",
+                "            elif v == \"median\":\n",
+                "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.median())\" % (k, k))\n",
+                "            elif v == \"count\":\n",
+                "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.count())\" % (k, k))\n",
+                "        #print(\"commands\", commands)\n",
+                "        commands.append(\"    df = pd.DataFrame(df_contents)\")\n",
+                "        return \"\\n\".join(commands)\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `dcef-0.2/package.json` & `dcef-0.2.1/package.json`

 * *Files identical despite different names*

### Comparing `dcef-0.2/tryit.ipynb` & `dcef-0.2.1/introduction.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9233928571428571%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'from dcef.dcef_widget import DCEFWidget')], delete: [3, "*

 * *            '2, 1]}}, 1: {\'source\': {insert: [(0, "df = '*

 * *            'pd.read_csv(\'./examples/data/2014-01-citibike-tripdata.csv\')\\n"), (1, \'w = '*

 * *            "DCEFWidget(df)\\n')], delete: [0]}}, 2: {'source': ['from dcef.all_transforms import "*

 * *            "Transform\\n', 'from dcef.lispy import s\\n', '#Here we start adding commands to the "*

 * *            "DCF Widget.  Every call to add_command repla […]*

```diff
@@ -3,93 +3,37 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
-                "import json\n",
-                "import numpy as np\n",
-                "from dcf.dcf_widget import DCFWidget"
+                "from dcef.dcef_widget import DCEFWidget"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = pd.read_csv('./examples/data/2014-01-citibike-tripdata.csv')\n",
-                "df2 = pd.read_csv('./examples/data/yellow_tripdata_2021-02.csv')"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "w = DCFWidget(df=df2)\n",
+                "w = DCEFWidget(df)\n",
                 "w"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "transformed_df = w.dcf_transform(w.commands, w.df)\n",
-                "w.transformed_df = json.loads(transformed_df.to_json(orient='table', indent=2))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "w.commands"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "w.generated_py_code"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "w.generated_py_code = w.dcf_to_py_core(w.commands[1:])\n",
-                "w.generated_py_code"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from dcf.all_transforms import Transform\n",
-                "from dcf.lispy import s"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
+                "from dcef.all_transforms import Transform\n",
+                "from dcef.lispy import s\n",
+                "#Here we start adding commands to the DCF Widget.  Every call to add_command replaces a command with the same name\n",
                 "@w.add_command\n",
                 "class GroupBy2(Transform):\n",
                 "    command_default = [s(\"groupby2\"), s('df'), 'col', {}]\n",
                 "    command_pattern = [[3, 'colMap', 'colEnum', ['null', 'sum', 'mean', 'median', 'count']]]\n",
                 "    @staticmethod \n",
                 "    def transform(df, col, col_spec):\n",
                 "        grps = df.groupby(col)\n",
@@ -101,20 +45,14 @@
                 "                df_contents[k] = grps[k].apply(lambda x: x.mean())\n",
                 "            elif v == \"median\":\n",
                 "                df_contents[k] = grps[k].apply(lambda x: x.median())\n",
                 "            elif v == \"count\":\n",
                 "                df_contents[k] = grps[k].apply(lambda x: x.count())\n",
                 "        return pd.DataFrame(df_contents)\n",
                 "\n",
-                "    #test_df = group_df\n",
-                "    #test_sequence = [s(\"groupby2\"), s('df'), 'c', dict(a='sum', b='mean')]\n",
-                "    test_output = pd.DataFrame(\n",
-                "        {'a':[100, 110], 'b':[2.5, 5.5]},\n",
-                "        index=['q','w'])\n",
-                "\n",
                 "    @staticmethod \n",
                 "    def transform_to_py(df, col, col_spec):\n",
                 "        commands = [\n",
                 "            \"    grps = df.groupby('%s')\" % col,\n",
                 "            \"    df_contents = {}\"\n",
                 "        ]\n",
                 "        for k, v in col_spec.items():\n",
@@ -122,18 +60,26 @@
                 "                commands.append(\"    paddydf_contents['%s'] = grps['%s'].apply(lambda x: x.sum())\" % (k, k))\n",
                 "            elif v == \"mean\":\n",
                 "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.mean())\" % (k, k))\n",
                 "            elif v == \"median\":\n",
                 "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.median())\" % (k, k))\n",
                 "            elif v == \"count\":\n",
                 "                commands.append(\"    df_contents['%s'] = grps['%s'].apply(lambda x: x.count())\" % (k, k))\n",
-                "        #print(\"commands\", commands)\n",
                 "        commands.append(\"    df = pd.DataFrame(df_contents)\")\n",
                 "        return \"\\n\".join(commands)\n"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# notice that there is now a Groupby2 Command in the widget"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -144,13 +90,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.2"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `dcef-0.2/tsconfig.json` & `dcef-0.2.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dcef-0.2/video_script.txt` & `dcef-0.2.1/video_script.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2/webpack.config.js` & `dcef-0.2.1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2/yarn.lock` & `dcef-0.2.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `dcef-0.2/dcf/all_transforms.py` & `dcef-0.2.1/dcef/all_transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .lispy import s
-from .configure_utils import configure_dcf
+from .configure_utils import configure_dcef
 import pandas as pd
 import numpy as np
 
 class Transform(object):
     pass
     
 class FillNA(Transform):
@@ -121,24 +121,9 @@
         return "\n".join(commands)
     
 
 
     
 
 DefaultCommandKlsList = [FillNA, DropCol, OneHot, GroupBy]
-# command_defaults, command_patterns, dcf_transform, dcf_to_py_core = configure_dcf([
-#     FillNA, DropCol, OneHot, GroupBy, SafeInt])
-command_defaults, command_patterns, dcf_transform, dcf_to_py_core = configure_dcf(DefaultCommandKlsList)
-
-#print(dcf_to_py_core([GroupBy.test_sequence]))
-#print(GroupBy.test_output)
-#todo, build in testing into the the classes at the time something is added to configure_dcf
-#print(dcf_transform(GroupBy.test_sequence, GroupBy.test_df))
-
-
-# class MakeCategorical(Transform):
-#     t_type = TransformType.column
-#     arguments = [Arguments.df, Arguments.column_name]
-#     command_template = [s('make-categorical'), s('df'), "col"]
-    
-
+command_defaults, command_patterns, dcef_transform, dcef_to_py_core = configure_dcef(DefaultCommandKlsList)
```

### Comparing `dcef-0.2/dcf/configure_utils.py` & `dcef-0.2.1/dcef/configure_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from .lispy import make_interpreter
-def configure_dcf(transforms):
+def configure_dcef(transforms):
     command_defaults = {}
     command_patterns = {}
 
     transform_lisp_primitives = {}
     to_py_lisp_primitives = {}
     for T in transforms:
         t = T()
         transform_name = t.command_default[0]['symbol']
         command_defaults[transform_name] = t.command_default
         command_patterns[transform_name] = t.command_pattern
         transform_lisp_primitives[transform_name] = T.transform
         to_py_lisp_primitives[transform_name] = T.transform_to_py
     
-    dcf_eval, raw_parse = make_interpreter(transform_lisp_primitives)
-    def dcf_transform(instructions, df):
+    dcef_eval, raw_parse = make_interpreter(transform_lisp_primitives)
+    def dcef_transform(instructions, df):
         df_copy = df.copy()
-        ret_val =  dcf_eval(instructions, {'df':df_copy})
+        ret_val =  dcef_eval(instructions, {'df':df_copy})
         #print(ret_val)
         return ret_val
 
     convert_to_python, __unused = make_interpreter(to_py_lisp_primitives)
-    def dcf_to_py(instructions):
+    def dcef_to_py(instructions):
         #I would prefer to implement this with a macro named something
         #like 'clean' that is implemented for the _convert_to_python
         #interpreter to return a string code block, and for the real DCF
         #interpreter as 'begin'... that way the exact same instructions
         #could be sent to either interpreter.  For now, this will do
         individual_instructions =  [x for x in map(lambda x:convert_to_python(x, {'df':5}), instructions)]
         #print("individual_instructions", individual_instructions)
         code_block =  '\n'.join(individual_instructions)
 
         return "def clean(df):\n" + code_block
-    return command_defaults, command_patterns, dcf_transform, dcf_to_py
+    return command_defaults, command_patterns, dcef_transform, dcef_to_py
```

### Comparing `dcef-0.2/dcf/dcf_transform.py` & `dcef-0.2.1/dcef/dcf_transform.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2/dcf/dcf_widget.py` & `dcef-0.2.1/dcef/dcef_widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 """
 TODO: Add module docstring
 """
 
 from ipywidgets import DOMWidget
 from traitlets import Unicode, List, Dict, observe
 from ._frontend import module_name, module_version
-from .all_transforms import configure_dcf, DefaultCommandKlsList
+from .all_transforms import configure_dcef, DefaultCommandKlsList
 import json
 
 
-class DCFWidget(DOMWidget):
+class DCEFWidget(DOMWidget):
     """TODO: Add docstring here
     """
     _model_name = Unicode('DCFWidgetModel').tag(sync=True)
     _model_module = Unicode(module_name).tag(sync=True)
     _model_module_version = Unicode(module_version).tag(sync=True)
     _view_name = Unicode('DCFWidgetView').tag(sync=True)
     _view_module = Unicode(module_name).tag(sync=True)
@@ -62,46 +62,27 @@
             if len(operations) == 1:
 
                 results['transformed_df'] = self.js_df
                 results['generated_py_code'] = 'no operations'
                 print('exiting early')
                 return
             
-            transformed_df = self.dcf_transform(operations, self.df)
+            transformed_df = self.dcef_transform(operations, self.df)
             results['transformed_df'] = json.loads(transformed_df.to_json(orient='table', indent=2))
 
-            results['generated_py_code'] = self.dcf_to_py_core(operations[1:])
+            results['generated_py_code'] = self.dcef_to_py_core(operations[1:])
             self.operation_results = results
             print("operations_results", results.keys())
         except Exception as e:
             print("error_setting", e)
             self.transform_error = str(e)
             raise
-            
-            
-    # @observe('commands')
-    # def interpret_commands(self, change):
-    #     try:
-    #         commands = change['new']
-    #         if len(commands) == 1:
-    #             self.transform_error = "matched"
-    #             self.transformed_df = self.js_df
-    #             return
-    #         transformed_df = self.dcf_transform(commands, self.df)
-    #         self.transformed_df = json.loads(transformed_df.to_json(orient='table', indent=2))
-    #         self.transform_error = ''
-    #         self.generated_py_code = self.dcf_to_py_core(commands[1:])
-    #         self.send_state()
-    #         print("interpret_to_py_code", commands)
-    #     except Exception as e:
-    #         self.transform_error = str(e)
-    #         self.generated_py_error = str(e)
 
     def setup_from_command_kls_list(self):
-        command_defaults, command_patterns, self.dcf_transform, self.dcf_to_py_core = configure_dcf(
+        command_defaults, command_patterns, self.dcef_transform, self.dcef_to_py_core = configure_dcef(
             self.command_classes)
         self.command_config = dict(
             argspecs=command_patterns, defaultArgs=command_defaults)
 
 
     def add_command(self, incomingCommandKls):
         without_incoming = [x for x in self.command_classes if not x.__name__ == incomingCommandKls.__name__]
```

### Comparing `dcef-0.2/dcf/df_methods.py` & `dcef-0.2.1/dcef/df_methods.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2/dcf/index.html` & `dcef-0.2.1/dcef/index.html`

 * *Files identical despite different names*

### Comparing `dcef-0.2/dcf/lispy.py` & `dcef-0.2.1/dcef/lispy.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2/dcf/views.py` & `dcef-0.2.1/dcef/views.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2/dcf/noarch/index.html` & `dcef-0.2.1/dcef/noarch/index.html`

 * *Files identical despite different names*

### Comparing `dcef-0.2/docs/source/_static/embed-bundle.js.LICENSE.txt` & `dcef-0.2.1/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/__init__.py` & `dcef-0.2.1/ipydatagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/paddy_widget.py` & `dcef-0.2.1/ipydatagrid/paddy_widget.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/labextension/package.json` & `dcef-0.2.1/ipydatagrid/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99921875%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7f7af2d8c54c49567ac4.js'}}"}*

```diff
@@ -61,15 +61,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/Bloomberg/ipydatagrid",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8a6d805ad1f7bc974c84.js"
+            "load": "static/remoteEntry.7f7af2d8c54c49567ac4.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./ipydatagrid/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `dcef-0.2/ipydatagrid/labextension/static/116.e2ccbe733d0a9edd1777.js` & `dcef-0.2.1/ipydatagrid/labextension/static/116.e2ccbe733d0a9edd1777.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/labextension/static/116.e2ccbe733d0a9edd1777.js.LICENSE.txt` & `dcef-0.2.1/ipydatagrid/labextension/static/116.e2ccbe733d0a9edd1777.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/labextension/static/250.970b486f665683a12362.js` & `dcef-0.2.1/ipydatagrid/labextension/static/250.970b486f665683a12362.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/labextension/static/250.970b486f665683a12362.js.LICENSE.txt` & `dcef-0.2.1/ipydatagrid/labextension/static/250.970b486f665683a12362.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/labextension/static/480.a1fc9bd0ae29c3af7210.js` & `dcef-0.2.1/ipydatagrid/labextension/static/480.a1fc9bd0ae29c3af7210.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/labextension/static/486.3a86dcecb5e722e84edc.js` & `dcef-0.2.1/ipydatagrid/labextension/static/486.3a86dcecb5e722e84edc.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/labextension/static/568.c9e5ec7d47bb9db3ae77.js` & `dcef-0.2.1/ipydatagrid/labextension/static/568.c9e5ec7d47bb9db3ae77.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/labextension/static/remoteEntry.8a6d805ad1f7bc974c84.js` & `dcef-0.2.1/ipydatagrid/labextension/static/remoteEntry.7f7af2d8c54c49567ac4.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, i, d, l, u, s, f, c, p, h, v, g, b, m = {
-            4607: (e, r, t) => {
+            8699: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(250), t.e(41), t.e(568)]).then((() => () => t(1568))),
                         "./extension": () => Promise.all([t.e(250), t.e(41), t.e(480)]).then((() => () => t(4480)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -284,10 +284,10 @@
                     d && d(w)
                 }
                 for (r && r(t); l < o.length; l++) n = o[l], w.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunkipydatagrid = self.webpackChunkipydatagrid || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), w.nc = void 0;
-    var S = w(4607);
+    var S = w(8699);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipydatagrid = S
 })();
```

### Comparing `dcef-0.2/ipydatagrid/labextension/static/third-party-licenses.json` & `dcef-0.2.1/ipydatagrid/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/nbextension/index.js` & `dcef-0.2.1/ipydatagrid/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/nbextension/index.js.LICENSE.txt` & `dcef-0.2.1/ipydatagrid/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2/ipydatagrid/nbextension/index.js.map` & `dcef-0.2.1/ipydatagrid/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `dcef-0.2/js/dcfwidget.ts` & `dcef-0.2.1/js/dcfwidget.ts`

 * *Files identical despite different names*

### Comparing `dcef-0.2/js/extension.ts` & `dcef-0.2.1/js/extension.ts`

 * *Files identical despite different names*

### Comparing `dcef-0.2/js/paddywidget.ts` & `dcef-0.2.1/js/paddywidget.ts`

 * *Files identical despite different names*

### Comparing `dcef-0.2/js/plugin.ts` & `dcef-0.2.1/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `dcef-0.2/.gitignore` & `dcef-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dcef-0.2/LICENSE.txt` & `dcef-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2/README.md` & `dcef-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# Data Cleaning Framework
-We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Data Cleaning Framework  (DCF) makes all of that better by providing a visual UI for common cleaning operations AND emitting python code that performs the transformation. Specifically, the DCF is a tool built to interactively explore, clean, and transform pandas dataframes.
+# DCEF - Data Cleaning Exploration Framework
+We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Data Cleaning Explorationg Framework  (DCEF) makes all of that better by providing a visual UI for common cleaning operations AND emitting python code that performs the transformation. Specifically, the DCEF is a tool built to interactively explore, clean, and transform pandas dataframes.
 
-![Data Cleaning Framework Screenshot](static/images/Dcf-tabbed.png)
+![Data Cleaning Exploration Framework Screenshot](static/images/dcf-jupyter.png)
 
 
 ## Installation
 
-If using JupyterLab, `dcf` requires JupyterLab version 3 or higher.
+If using JupyterLab, `dcef` requires JupyterLab version 3 or higher.
 
-You can install `dcf` using `pip` or `conda`:
+You can install `dcef` using `pip`
 
 Using `pip`:
 
 ```bash
-pip install -i https://test.pypi.org/simple/ dcf==0.1.1
+pip install dcef
 ```
 
 ## Caveats
-DCF is in beta form.  At this point, it is based on from Bloomberg's [ipydatagrid](https://github.com/bloomberg/ipydatagrid) for the basis of the widget build.
+DCEF is in beta form.  At this point, it is based on from Bloomberg's [ipydatagrid](https://github.com/bloomberg/ipydatagrid) for the basis of the widget build.
 
-If you install ipydatagrid with dcf at this point, expect errors.
+If you install ipydatagrid with dcef at this point, expect errors.
 
 
 
-# Using DCF
+# Using DCEF
 
 in a jupylter notebook just add the following to a cell
 
 ```python
-from dcf.dcf_widget import DCFWidget
-DCFWidget(df=df)  #df being the dataframe you want to explore
+from dcef.dcef_widget import DCEFWidget
+DCEFWidget(df=df)  #df being the dataframe you want to explore
 ``` 
-and you will see the UI for DCF
+and you will see the UI for DCEF
 
 
 ## Using commands
 
-At the core DCF commands operate on columns.  You must first click on a cell (not a header) in the top pane to select a column.
+At the core DCEF commands operate on columns.  You must first click on a cell (not a header) in the top pane to select a column.
 
 Next you must click on a command like `dropcol`, `fillna`, or `groupby` to create a new command
 
 After creating a new command, you will see that command in the commands list, now you must edit the details of a command.  Select the command by clicking on the bottom cell.
 
 At this point you can either delete the command by clicking the `X` button or change command parameters.
 
 ## Writing your own commands
 
-Builtin commands are found in [all_transforms.py](dcf/all_transforms.py)
+Builtin commands are found in [all_transforms.py](dcef/all_transforms.py)
 
 ### Simple example
 Here is a simple example command
 ```python
 class DropCol(Transform):
     command_default = [s('dropcol'), s('df'), "col"]
     command_pattern = [None]
@@ -138,15 +138,15 @@
 These transforms emit multiple DataFrames
   * Relational extract (extract one or more columns into a second dataframe that can be joined back to a foreign key column)
   * Split on column (emit separate dataframes for each value of a categorical, no shape editting)
 * DataFrame combination
   * concat (concatenate multiple dataframes, with UI affordances to assure a similar shape)
   * join (join two dataframes on a key, with UI affordances)
 
-DCF can only work on a single input dataframe shape at a time.  Any newly created columns are visible on output, but not available for manipulation in the same DCF Cell.
+DCEF can only work on a single input dataframe shape at a time.  Any newly created columns are visible on output, but not available for manipulation in the same DCEF Cell.
 
 
 # Components
 * a rich table widget that is embeddable into applications and in the jupyter notebook.
 * A UI for selecting and trying transforms interactively
 * An output table widget showing the transformed dataframe
 
@@ -155,23 +155,23 @@
 
 ## Exists now
   * React frontend app
     * Displays a datatframe
 	* Simple UI for column level functions
 	* Shows generated python code
 	* Shows transformed data frame
-  * DCF server
+  * DCEF server
     * Serves up dataframes for use by frontend
-	* responds to dcf commands
+	* responds to dcef commands
 	* shows generated python code
   * Developer User experience
-	* define DCF commands in python onloy
-  * DCF Intepreter
+	* define DCEF commands in python onloy
+  * DCEF Intepreter
     * Based on Peter Norvig's lispy.py, a simple syntax that is easy for the frontend to generate (no parens, just JSON arrays)
-  * DCF core (actual transforms supported)
+  * DCEF core (actual transforms supported)
     * dropcol
 	* fillna
 	* one hot
 	* safe int
 	* GroupBy
 
 ## Next major features
@@ -183,76 +183,37 @@
     * Styling
 	  * Server only, some UI for DataFrame selection
     * Pre filtering concept (only operate on first 1000 rows, some sample of all rows)
 	* DataFrame joining UI
 	* Summary statistics tab for incoming dataframe
 	* Multi index columns
 	* DateTimeIndex support
-  * DCF core
+  * DCEF core
 	* MakeCategorical
 	* Quantize
 	* Resample
 	* ManyColdDecoding
 	* IndexShift
 	* Computed
 	* Stack/Unstack
 	* RelationalExtract
 	* Split
 	* concat
 	* join
 	
-# FAQ
-## Why did you use LISP?
-
-This is a problem domain that requried a DSL and intermediate language.  I could have written my own or chosen an existing language.  I chose LISP because it is simple to interpret and generate, additionally it is well understood.  Yes LISP is obscure, but it is less obscure than a custom language I would write myself.  I didn't want to expose an entire progrmaming language with all the attendant security risks, I wanted a small safe strict subset of programming features that I explicitly exposed.  LISP is easier to manipulate as an AST than any language in PL history.  I am not yet using any symbolic manipulation facilities of LISP, and will probably only use them in limited ways. 
-
-## Do I need to know LISP to use DCF?
-
-No.  Users of DCF will never need to know that LISP is at the core of the system.
-
-## Do I need to know LISP to contribute to DCF?
-
-Not really.  Transfrom functions and their python equivalent are added to the dcf interpreter.  Transform functions are very simple and straight forward.  Here are the two functions that make `fillna` work.
-```
-def fillna(df, col, val):
-    df.fillna({col:val}, inplace=True)
-    return df
-
-def fillna_py(df, col, val):
-    return "    df.fillna({'%s':%r}, inplace=True)" % (col, val)
-```
-
-If you want to work on code transformations, then a knowledge of lisp and particularly lisp macros are helpful.
-
-## What is an example of a code transformation?
-
-Imagine you have a `dropcol` command which takes a single column to drop, also imagine that there is a function `dropcols` which takes a list of columns to drop.
-
-It is easier to build the UI to emit individual `dropcol` commands, you will end up with more readable code when you have a single command that drops all columns.
-
-You could write a transform which reads all `dropcol` forms and rewrites it to a single `dropcols` command.
-
-Alternatively, you could write a command that instead of subtractively reducing a dataframe, builds up a new dataframe from an explicit list of columns.  That is also a type of transform that could be written.
-
-## Is DCF meant to repalce knowledge of python/pandas 
-
-No, DCF helps experienced pandas devs quickly build and try the transformations they already know.  Transformation names stay very close to the underlying pandas names.  DCF makes different transforms more discoverable than reading obscure blogposts and half working stackoverflow submissions.  Different transformations can be quickly tried without a lot of reading and tinkering to see if it is the transform you want.  Finally, all transformations are emitted as python code.  That python code can be a starting point.
-
-
-
 
 
 
 ## Development installation
 
 For a development installation:
 
 ```bash
-git clone https://github.com/paddymul/dcf.git
-cd dcf
+git clone https://github.com/paddymul/dcef.git
+cd dcef
 conda install ipywidgets=8 jupyterlab
 pip install -ve .
 ```
 
 Enabling development install for Jupyter notebook:
```

### Comparing `dcef-0.2/pyproject.toml` & `dcef-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9"
 ]
-version = "0.2"
+version = "0.2.1"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "nbval>=0.9",
```

### Comparing `dcef-0.2/PKG-INFO` & `dcef-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcef
-Version: 0.2
+Version: 0.2.1
 Summary: Data Cleaning Framework - UI for quickly cleaning pandas dataframes 
 Project-URL: Homepage, https://github.com/bloomberg/ipydatagrid
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -49,63 +49,63 @@
 Provides-Extra: test
 Requires-Dist: nbval>=0.9; extra == 'test'
 Requires-Dist: pandas<=1.3.5; extra == 'test'
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
-# Data Cleaning Framework
-We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Data Cleaning Framework  (DCF) makes all of that better by providing a visual UI for common cleaning operations AND emitting python code that performs the transformation. Specifically, the DCF is a tool built to interactively explore, clean, and transform pandas dataframes.
+# DCEF - Data Cleaning Exploration Framework
+We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Data Cleaning Explorationg Framework  (DCEF) makes all of that better by providing a visual UI for common cleaning operations AND emitting python code that performs the transformation. Specifically, the DCEF is a tool built to interactively explore, clean, and transform pandas dataframes.
 
-![Data Cleaning Framework Screenshot](static/images/Dcf-tabbed.png)
+![Data Cleaning Exploration Framework Screenshot](static/images/dcf-jupyter.png)
 
 
 ## Installation
 
-If using JupyterLab, `dcf` requires JupyterLab version 3 or higher.
+If using JupyterLab, `dcef` requires JupyterLab version 3 or higher.
 
-You can install `dcf` using `pip` or `conda`:
+You can install `dcef` using `pip`
 
 Using `pip`:
 
 ```bash
-pip install -i https://test.pypi.org/simple/ dcf==0.1.1
+pip install dcef
 ```
 
 ## Caveats
-DCF is in beta form.  At this point, it is based on from Bloomberg's [ipydatagrid](https://github.com/bloomberg/ipydatagrid) for the basis of the widget build.
+DCEF is in beta form.  At this point, it is based on from Bloomberg's [ipydatagrid](https://github.com/bloomberg/ipydatagrid) for the basis of the widget build.
 
-If you install ipydatagrid with dcf at this point, expect errors.
+If you install ipydatagrid with dcef at this point, expect errors.
 
 
 
-# Using DCF
+# Using DCEF
 
 in a jupylter notebook just add the following to a cell
 
 ```python
-from dcf.dcf_widget import DCFWidget
-DCFWidget(df=df)  #df being the dataframe you want to explore
+from dcef.dcef_widget import DCEFWidget
+DCEFWidget(df=df)  #df being the dataframe you want to explore
 ``` 
-and you will see the UI for DCF
+and you will see the UI for DCEF
 
 
 ## Using commands
 
-At the core DCF commands operate on columns.  You must first click on a cell (not a header) in the top pane to select a column.
+At the core DCEF commands operate on columns.  You must first click on a cell (not a header) in the top pane to select a column.
 
 Next you must click on a command like `dropcol`, `fillna`, or `groupby` to create a new command
 
 After creating a new command, you will see that command in the commands list, now you must edit the details of a command.  Select the command by clicking on the bottom cell.
 
 At this point you can either delete the command by clicking the `X` button or change command parameters.
 
 ## Writing your own commands
 
-Builtin commands are found in [all_transforms.py](dcf/all_transforms.py)
+Builtin commands are found in [all_transforms.py](dcef/all_transforms.py)
 
 ### Simple example
 Here is a simple example command
 ```python
 class DropCol(Transform):
     command_default = [s('dropcol'), s('df'), "col"]
     command_pattern = [None]
@@ -193,15 +193,15 @@
 These transforms emit multiple DataFrames
   * Relational extract (extract one or more columns into a second dataframe that can be joined back to a foreign key column)
   * Split on column (emit separate dataframes for each value of a categorical, no shape editting)
 * DataFrame combination
   * concat (concatenate multiple dataframes, with UI affordances to assure a similar shape)
   * join (join two dataframes on a key, with UI affordances)
 
-DCF can only work on a single input dataframe shape at a time.  Any newly created columns are visible on output, but not available for manipulation in the same DCF Cell.
+DCEF can only work on a single input dataframe shape at a time.  Any newly created columns are visible on output, but not available for manipulation in the same DCEF Cell.
 
 
 # Components
 * a rich table widget that is embeddable into applications and in the jupyter notebook.
 * A UI for selecting and trying transforms interactively
 * An output table widget showing the transformed dataframe
 
@@ -210,23 +210,23 @@
 
 ## Exists now
   * React frontend app
     * Displays a datatframe
 	* Simple UI for column level functions
 	* Shows generated python code
 	* Shows transformed data frame
-  * DCF server
+  * DCEF server
     * Serves up dataframes for use by frontend
-	* responds to dcf commands
+	* responds to dcef commands
 	* shows generated python code
   * Developer User experience
-	* define DCF commands in python onloy
-  * DCF Intepreter
+	* define DCEF commands in python onloy
+  * DCEF Intepreter
     * Based on Peter Norvig's lispy.py, a simple syntax that is easy for the frontend to generate (no parens, just JSON arrays)
-  * DCF core (actual transforms supported)
+  * DCEF core (actual transforms supported)
     * dropcol
 	* fillna
 	* one hot
 	* safe int
 	* GroupBy
 
 ## Next major features
@@ -238,76 +238,37 @@
     * Styling
 	  * Server only, some UI for DataFrame selection
     * Pre filtering concept (only operate on first 1000 rows, some sample of all rows)
 	* DataFrame joining UI
 	* Summary statistics tab for incoming dataframe
 	* Multi index columns
 	* DateTimeIndex support
-  * DCF core
+  * DCEF core
 	* MakeCategorical
 	* Quantize
 	* Resample
 	* ManyColdDecoding
 	* IndexShift
 	* Computed
 	* Stack/Unstack
 	* RelationalExtract
 	* Split
 	* concat
 	* join
 	
-# FAQ
-## Why did you use LISP?
-
-This is a problem domain that requried a DSL and intermediate language.  I could have written my own or chosen an existing language.  I chose LISP because it is simple to interpret and generate, additionally it is well understood.  Yes LISP is obscure, but it is less obscure than a custom language I would write myself.  I didn't want to expose an entire progrmaming language with all the attendant security risks, I wanted a small safe strict subset of programming features that I explicitly exposed.  LISP is easier to manipulate as an AST than any language in PL history.  I am not yet using any symbolic manipulation facilities of LISP, and will probably only use them in limited ways. 
-
-## Do I need to know LISP to use DCF?
-
-No.  Users of DCF will never need to know that LISP is at the core of the system.
-
-## Do I need to know LISP to contribute to DCF?
-
-Not really.  Transfrom functions and their python equivalent are added to the dcf interpreter.  Transform functions are very simple and straight forward.  Here are the two functions that make `fillna` work.
-```
-def fillna(df, col, val):
-    df.fillna({col:val}, inplace=True)
-    return df
-
-def fillna_py(df, col, val):
-    return "    df.fillna({'%s':%r}, inplace=True)" % (col, val)
-```
-
-If you want to work on code transformations, then a knowledge of lisp and particularly lisp macros are helpful.
-
-## What is an example of a code transformation?
-
-Imagine you have a `dropcol` command which takes a single column to drop, also imagine that there is a function `dropcols` which takes a list of columns to drop.
-
-It is easier to build the UI to emit individual `dropcol` commands, you will end up with more readable code when you have a single command that drops all columns.
-
-You could write a transform which reads all `dropcol` forms and rewrites it to a single `dropcols` command.
-
-Alternatively, you could write a command that instead of subtractively reducing a dataframe, builds up a new dataframe from an explicit list of columns.  That is also a type of transform that could be written.
-
-## Is DCF meant to repalce knowledge of python/pandas 
-
-No, DCF helps experienced pandas devs quickly build and try the transformations they already know.  Transformation names stay very close to the underlying pandas names.  DCF makes different transforms more discoverable than reading obscure blogposts and half working stackoverflow submissions.  Different transformations can be quickly tried without a lot of reading and tinkering to see if it is the transform you want.  Finally, all transformations are emitted as python code.  That python code can be a starting point.
-
-
-
 
 
 
 ## Development installation
 
 For a development installation:
 
 ```bash
-git clone https://github.com/paddymul/dcf.git
-cd dcf
+git clone https://github.com/paddymul/dcef.git
+cd dcef
 conda install ipywidgets=8 jupyterlab
 pip install -ve .
 ```
 
 Enabling development install for Jupyter notebook:
```

