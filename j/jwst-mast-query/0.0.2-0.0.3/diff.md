# Comparing `tmp/jwst_mast_query-0.0.2.tar.gz` & `tmp/jwst_mast_query-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwst_mast_query-0.0.2.tar", last modified: Fri Mar 24 18:09:45 2023, max compression
+gzip compressed data, was "jwst_mast_query-0.0.3.tar", last modified: Fri Apr 21 17:08:19 2023, max compression
```

## Comparing `jwst_mast_query-0.0.2.tar` & `jwst_mast_query-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-03-24 18:09:45.616971 jwst_mast_query-0.0.2/
--rw-r--r--   0 hilbert   (3978) staff       (20)     2366 2022-03-04 20:55:11.000000 jwst_mast_query-0.0.2/.gitignore
--rw-r--r--   0 hilbert   (3978) staff       (20)     1127 2023-03-24 17:58:44.000000 jwst_mast_query-0.0.2/CHANGES.rst
--rw-r--r--   0 hilbert   (3978) staff       (20)     4528 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 hilbert   (3978) staff       (20)     1553 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.2/LICENSE.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)      848 2023-03-24 18:09:45.616622 jwst_mast_query-0.0.2/PKG-INFO
--rw-r--r--   0 hilbert   (3978) staff       (20)    37902 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.2/README.md
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-03-24 18:09:45.611677 jwst_mast_query-0.0.2/jwst_mast_query/
--rw-r--r--   0 hilbert   (3978) staff       (20)       89 2022-02-16 16:07:13.000000 jwst_mast_query-0.0.2/jwst_mast_query/__init__.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     8183 2023-03-23 16:57:21.000000 jwst_mast_query-0.0.2/jwst_mast_query/jwst_download.py
--rw-r--r--   0 hilbert   (3978) staff       (20)     7859 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.2/jwst_mast_query/jwst_query.cfg
--rwxr-xr-x   0 hilbert   (3978) staff       (20)    73151 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.2/jwst_mast_query/jwst_query.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)    59698 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.2/jwst_mast_query/pdastro.py
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-03-24 18:09:45.615023 jwst_mast_query-0.0.2/jwst_mast_query/scripts/
--rw-r--r--   0 hilbert   (3978) staff       (20)     1701 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.2/jwst_mast_query/scripts/jwst_download.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     8605 2023-03-10 17:35:18.000000 jwst_mast_query-0.0.2/jwst_mast_query/sortable.js
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-03-24 18:09:45.615518 jwst_mast_query-0.0.2/jwst_mast_query/utils/
--rw-r--r--   0 hilbert   (3978) staff       (20)      509 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.2/jwst_mast_query/utils/constants.py
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-03-24 18:09:45.614413 jwst_mast_query-0.0.2/jwst_mast_query.egg-info/
--rw-r--r--   0 hilbert   (3978) staff       (20)      848 2023-03-24 18:09:45.000000 jwst_mast_query-0.0.2/jwst_mast_query.egg-info/PKG-INFO
--rw-r--r--   0 hilbert   (3978) staff       (20)      534 2023-03-24 18:09:45.000000 jwst_mast_query-0.0.2/jwst_mast_query.egg-info/SOURCES.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)        1 2023-03-24 18:09:45.000000 jwst_mast_query-0.0.2/jwst_mast_query.egg-info/dependency_links.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)      184 2023-03-24 18:09:45.000000 jwst_mast_query-0.0.2/jwst_mast_query.egg-info/requires.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)       16 2023-03-24 18:09:45.000000 jwst_mast_query-0.0.2/jwst_mast_query.egg-info/top_level.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)       98 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.2/pyproject.toml
--rw-r--r--   0 hilbert   (3978) staff       (20)       38 2023-03-24 18:09:45.617159 jwst_mast_query-0.0.2/setup.cfg
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     2828 2023-03-23 16:57:21.000000 jwst_mast_query-0.0.2/setup.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.301061 jwst_mast_query-0.0.3/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     2366 2022-03-04 20:55:11.000000 jwst_mast_query-0.0.3/.gitignore
+-rw-r--r--   0 hilbert   (3978) staff       (20)     1822 2023-04-21 16:52:11.000000 jwst_mast_query-0.0.3/CHANGES.rst
+-rw-r--r--   0 hilbert   (3978) staff       (20)     4528 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 hilbert   (3978) staff       (20)     1553 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.3/LICENSE.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)      848 2023-04-21 17:08:19.300738 jwst_mast_query-0.0.3/PKG-INFO
+-rw-r--r--   0 hilbert   (3978) staff       (20)    39611 2023-04-14 18:08:15.000000 jwst_mast_query-0.0.3/README.md
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.295932 jwst_mast_query-0.0.3/jwst_mast_query/
+-rw-r--r--   0 hilbert   (3978) staff       (20)       89 2022-02-16 16:07:13.000000 jwst_mast_query-0.0.3/jwst_mast_query/__init__.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     8183 2023-03-23 16:57:21.000000 jwst_mast_query-0.0.3/jwst_mast_query/jwst_download.py
+-rw-r--r--   0 hilbert   (3978) staff       (20)     8205 2023-04-14 18:08:15.000000 jwst_mast_query-0.0.3/jwst_mast_query/jwst_query.cfg
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)    91453 2023-04-21 16:44:21.000000 jwst_mast_query-0.0.3/jwst_mast_query/jwst_query.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)    59698 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.3/jwst_mast_query/pdastro.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.299015 jwst_mast_query-0.0.3/jwst_mast_query/scripts/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     1765 2023-04-04 21:08:28.000000 jwst_mast_query-0.0.3/jwst_mast_query/scripts/jwst_download.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     8605 2023-03-10 17:35:18.000000 jwst_mast_query-0.0.3/jwst_mast_query/sortable.js
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.299762 jwst_mast_query-0.0.3/jwst_mast_query/utils/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     3885 2023-04-17 16:28:47.000000 jwst_mast_query-0.0.3/jwst_mast_query/utils/constants.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.298637 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/
+-rw-r--r--   0 hilbert   (3978) staff       (20)      848 2023-04-21 17:08:18.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/PKG-INFO
+-rw-r--r--   0 hilbert   (3978) staff       (20)      534 2023-04-21 17:08:19.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/SOURCES.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)        1 2023-04-21 17:08:18.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/dependency_links.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)      184 2023-04-21 17:08:18.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/requires.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)       16 2023-04-21 17:08:18.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/top_level.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)       98 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.3/pyproject.toml
+-rw-r--r--   0 hilbert   (3978) staff       (20)       38 2023-04-21 17:08:19.301226 jwst_mast_query-0.0.3/setup.cfg
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     2828 2023-03-23 16:57:21.000000 jwst_mast_query-0.0.3/setup.py
```

### Comparing `jwst_mast_query-0.0.2/.gitignore` & `jwst_mast_query-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.2/CODE_OF_CONDUCT.md` & `jwst_mast_query-0.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.2/LICENSE.txt` & `jwst_mast_query-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.2/PKG-INFO` & `jwst_mast_query-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwst_mast_query
-Version: 0.0.2
+Version: 0.0.3
 Summary: Query MAST for JWST products, and download them
 Home-page: https://github.com/spacetelescope/jwst_mast_query
 Author: STScI (Rest)
 Author-email: arest@stsci.edu
 License: UNKNOWN
 Keywords: astronomy
 Platform: UNKNOWN
```

### Comparing `jwst_mast_query-0.0.2/README.md` & `jwst_mast_query-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 - --lookbacktime : The number of days before the present to use as the beginning of the query
 
 - --propID : The JWST proposal number. e.g. `--propID 1409` or `--propID 01409`
 
 - --obsnums : Optional observation number or numbers within propID to retrieve. e.g. `--obsnums 3 103` would retrieve files only from observations 3 and 103.
 
-- --makewebpages : If set, an index.html file is generated, containing info and images of the retrieved data. Note that this option is not currently in the config file, and must be specified at the command line.
+- --makewebpages : Make webpages for the products for each propID containing info and images of the retrieved data.
 
 
 These are just a few of the options that can be set. The rest are specified in the config file provided in the call. Config file details are given below.
 For more example calls, see the **Examples** section below.
 
 
 ### Config File and Input Options
@@ -78,34 +78,44 @@
 | Parameter Name: default value                                                                       | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 |-----------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | instrument: nircam                                                                                  | Specify the instrument (nircam, nirspec, niriss, miri, fgs)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | propID                                                                                  | Specify the JWST proposal number to query for. This can be a 5 digit integer, or for a smaller number, an integer with or without prepended zeros. e.g. 1409 or 01409.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 | obsnums                                                                                  | Specify the observation numbers within the propID. This can be a single number, or a bracketed list of numbers. e.g. 3 or [3, 103]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 | outrootdir: $JWSTDOWNLOAD_OUTDIR                                                                    | The base directory for the downloaded products. This can be the name of an environment variable (such as JWSTDOWNLOAD_OUTDIR in this example), or a path. Note the preceding "$" in the case where an environment variable is given. If you include the --outrootdir command line argument when calling jwst_query.py or jwst_download.py, that value will override the value provided here.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 | outsubdir:                                                                                          | Any additional directory to add to the base directory. This can be used to customize the organization of the downloaded products.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| skip_propID2outsubdir: False                                                                        | Don't use the propID in the output directory. This can be used for custom output directory, e.g., to put the products from several APT files into one directory                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| skip_propID2outsubdir: False                                                                        | By default, the APT proposal ID is added as a subdir to the directory. You can skip this with this option.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | obsnum2outsubdir: True                                                                              | If True, the observation number will be used to create a subdirectory into which the appropriate files will be placed. e.g. $JWSTDOWNLOAD_OUTDIR/01410/obsnum23/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-| propIDs_obsnum2outsubdir: [1409]                                                                    | If True, only for the listed proposal numbers will observation numbers will be used to create a subdirectory into which the appropriate files will be placed. e.g. $JWSTDOWNLOAD_OUTDIR/01410/obsnum23/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-| skip_check_if_outfile_exists: False                                                                 | The script queries MAST for products, and then checks if each file already exists in the output directory or not ("dl_code" and "dl_str" columns). For large numbers of products, this can take time. By setting this option to True, this check can be skipped.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
+| propIDs_obsnum2outsubdir: [1409]                                                                    | Specify list of propID for which obsnum2outsubdir is True. Only for the listed proposal numbers will observation numbers be used to create a subdirectory into which the appropriate files will be placed. e.g. $JWSTDOWNLOAD_OUTDIR/01410/obsnum23/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| skip_check_if_outfile_exists: False                                                                 | By default, the script queries MAST for products, and then checks if each file already exists in the output directory or not ("dl_code" and "dl_str" columns). For large numbers of products, this can take time. By setting this option to True, this check can be skipped.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | Nobs_per_batch: 2                                                                                   | For large programs, the query for the products can time out, and in these cases it is better to split up the query into Nobs_per_batch observations per batch. For example, if there are 22 observations, and Nobs_per_batch=4, then there will be 6 batches, 5 batches with 4 observations, and the last batch with 2.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | obsmode: ['image', 'wfss']                                                                          | Optionally specify the observation modes to query for. If provided, MAST will be queried only for these types of observations. e.g. assuming instrument is 'nircam', obsmode: ['image', 'wfss'] will query MAST for NIRCAM/IMAGE and NIRCAM/WFSS data. If left empty, the query will include all modes. For a list of valid modes, see the example config file in the repository. Note that as of 24 March 2023, MAST is in the process of reprocessing all data to add the mode values to the instrument names. Until this process is complete, some older data may not include the mode name, and therefore will not be found via a query that includes the mode name.                                                                                                                                                                                                                                                                                                                                                                      |
 | filetypes: ['uncal']                                                                                | List of file types to select in the product table, e.g., \_uncal.fits or \_uncal.jpg. If no suffix is given, .fits is appended. If only letters, then \_ and .fits are added. For example, 'uncal' gets expanded to \_uncal.fits. Typical image filetypes are uncal, rate, rateints, cal. For downloading a single file type, the brackets must still surround the file suffix, as the script expects a list. A relatively complete list of options includes: ['\_segm.fits', '\_asn.json', '\_pool.csv', '\_i2d.jpg', '\_thumb.jpg', '\_cat.ecsv', '\_i2d.fits', '\_uncal.fits', '\_uncal.jpg', '\_cal.fits', '\_trapsfilled.fits', '\_cal.jpg', '\_rate.jpg', '\_rateints.jpg', '\_trapsfilled.jpg', '\_rate.fits', '\_rateints.fits'] See the [JWST calibration pipeline documentation](https://jwst-pipeline.readthedocs.io/en/latest/jwst/introduction.html#pipeline-step-suffix-definitions) for a complete list. |
+| jpg_separate_subdir: False                                                                          | If True, downloaded jpgs are saved in separate "jpg" subdirectories, along side the fits files.																					|
 | guidestars: False                                                                                   | If guidestars is set to True, guidestar products are also included. Note: there are a **lot** of guide star products. We recommend you set to True only if really needed!                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
 | lookbacktime: 1.0                                                                                   | Lookback time in days. The script will query MAST over a time from the lookback time to the present moment. Note that all other time parameters (date_select, etc) override the lookback time.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+| date_select: []                                                                                     | Specify date range (MJD or isot format) applied to "dateobs_center" column. If single value, then only exact matches will be returned. If a single value has "+" or "-" at the end, then it is a lower and upper limit, respectively. date_select will override the lookbacktime. Examples: 58400+, 58400-, 2020-11-23+,2020-11-23 2020-11-25                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| savetables:                                                                                         | Save the tables (selected products, obsTable, summary with suffix selprod.txt, obs.txt, summary.txt, respectively) with the specified string as basename. Tables are saved in the same output directory as the data.  If no string is provided, the tables are not saved.                                                                                                                                                                                                                                                                                                        |    
 | mastcolumns_obsTable: ['proposal_id', 'dataURL', 'obs_id', 't_min','t_exptime']                     | Core columns returned from MAST to the obsTable                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | outcolumns_productTable                                                                             | List of columns to be shown in product table, e.g., ['proposal_id', 'obsnum', 'obsID', 'parent_obsid', 'obs_id', 'dataproduct_type', 'productFilename', 'filetype', 'calib_level', 'size', 'outfilename', 'dl_code', 'dl_str']                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | outcolumns_obsTable: ['proposal_id', 'obsnum', 'obsid', 'obs_id', 't_min', 't_exptime', 'date_min'] | Output columns for the obsTable.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | sortcols_productTable: ['calib_level','filetype','obsID']                                           | The productTable is sorted based on these columns. The default sorts the table based on calibration level.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | sortcols_obsTable: ['date_min','proposal_id','obsnum']                                              | The obsTable is sorted based on these columns. The defaults sort the table in the order the observations were observed                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| sortcols_summaryTable: ['date_start','proposal_id','obsnum']                                        | The summary table is sorted based on these columns. The default sorts the table in the order the observations were observed                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| date_select: []                                                                                     | Specify date range (MJD or isot format) applied to "dateobs_center" column. If single value, then only exact matches will be returned. If a single value has "+" or "-" at the end, then it is a lower and upper limit, respectively. Examples: 58400+, 58400-, 2020-11-23+,2020-11-23 2020-11-25                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| savetables:                                                                                         | Save the tables (selected products, obsTable, summary with suffix selprod.txt, obs.txt, summary.txt, respectively) with the specified string as basename. Filenames will then be *xxxx.summary.txt*, *xxxx.obs.txt*, and *xxxx.selprod.txt*, where xxxx is the savetables value. Tables are saved in the same output directory as the data.  If no string is provided, the tables are not saved.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| webpage_thumbnail_width: 100                                                                        | Width in pixels of the resized jpg images to be inserted into the index.html summary file. |
-| webpage_thumbnail_height:                                                                           | Height in pixels of the resized jpg images to be inserted into the index.html summary file. If left undefined, the height will be determined from webpage_thumbnail_width and the aspect ratio of the original image.              |
-| webpage_level12_jpgs: ['\_uncal.jpg','\_dark.jpg','\_rate.jpg','\_rateints.jpg','\_trapsfilled.jpg','\_cal.jpg','\_crf.jpg'] | Filetypes whose thumbnails will be shown in index.html. |
+| sortcols_summaryTable: ['date_start','proposal_id','obsnum']                                        | The summary table is sorted based on these columns. The default sorts the table in the order the observations were observed                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                         |
+| makewebpages: False         																	       | Make webpages for the products for each propID containing info and images of the retrieved data.  |
+| webpage_tablefigsize_width: 																		   | Specify the figure box width. Recommended: 100-150, or don't specify if webpage_mkthumbnails is True. In that case the size of the thumbnails is used by default. |
+| webpage_tablefigsize_height: 																		   | Specify the figure box height. Recommended: 100-150, or don't specify if webpage_mkthumbnails is True. In that case the size of the thumbnails is used by default. |
+| webpage_level12_jpgs: ['\_uncal.jpg','\_dark.jpg','\_rate.jpg','\_rateints.jpg','\_trapsfilled.jpg','\_cal.jpg','\_crf.jpg'] | List of filetypes whose thumbnails will be shown in index.html. |
+| webpage_fitskeys2table: ['TARG_RA', 'TARG_DEC', 'FILTER', 'PUPIL', 'READPATT', 'NINTS', 'NGROUPS', 'NFRAMES', 'DATE-BEG', 'DATE-END', 'EFFINTTM', 'EFFEXPTM'] | List of fits header keywords that should be copied to the table. |
+| webpage_cols4table': ['proposal_id', 'obsnum', 'visit', 'obsID', 'parent_obsid', 'sca', 'FILTER', 'PUPIL', 'READPATT', 'uncal', 'dark', 'rate', 'rateints', 'cal', 'TARG_RA', 'TARG_DEC', 'NINTS', 'NGROUPS', 'NFRAMES', 'DATE-BEG', 'DATE-END', 'EFFINTTM', 'EFFEXPTM', 'size', 'obs_id', 'outfilename'] | Columns to be shown in index.html |
+| webpage_sortcols: ['proposal_id', 'obsnum', 'visit', 'sca']                                         | Columns to sort index.html by. |
+| webpage_mkthumbnails: True                                                                          | If True, a thumbnail jpg is created for each of the jpg products listed in webpage_level12_jpgs  |
+| webpage_thumbnails_overwrite: False                                                                 | If True, remake thumbnails even if they already exist |
+| webpage_thumbnails_width: 120                                                                        | Width in pixels of the resized jpg images to be inserted into the index.html summary file. |
+| webpage_thumbnails_height:                                                                           | Height in pixels of the resized jpg images to be inserted into the index.html summary file. If left undefined, the height will be determined from webpage_thumbnail_width and the aspect ratio of the original image.              |
+
 
 
 ## Outputs
 
 The primary output of **jwst_download.py** are the downloaded files themselves. By default, the downloaded files are saved into the directory:
 
 \<outrootdir\>\<outsubdir\>\<proposal number\>obsnum\<XX\>
```

### Comparing `jwst_mast_query-0.0.2/jwst_mast_query/jwst_download.py` & `jwst_mast_query-0.0.3/jwst_mast_query/jwst_download.py`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.2/jwst_mast_query/jwst_query.cfg` & `jwst_mast_query-0.0.3/jwst_mast_query/jwst_query.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,26 @@
 # The script first gets all observations for the given query. Then it queries all products for these
 # observations. For large programs, the query for the products can time out, and in these cases it
 # is better to split up the query into Nobs_per_batch observations per batch. For example, if there are
 # 22 observations, and Nobs_per_batch=4, then there will be 6 batches, 5 batches with 4 observations, and
 # the last batch with 2.
 Nobs_per_batch: 2
 
+# Specify the proposal ID to query for. Can be an integer, or a 5-digit string, e.g.
+# propID: 1068
+# propID: '01068'
+propID:
+
+# Optionally specify the observation numbers to query for. Can be a single integer or string, or a list
+# of integers or strings.
+# e.g. obsnums: 001
+# obsnums: 1
+# obsnums: [001, 002]
+obsnums:
+
 # Optionally specify the observation modes to query for. If provided, MAST will be queried only for these
 # types of observations. e.g. assuming instrument is 'nircam', obsmode: ['image', 'wfss'] will query MAST
 # for NIRCAM/IMAGE and NIRCAM/WFSS data. If left empty, the query will include all modes. Valid modes include:
 # miri: ['coron', 'ifu', 'image', 'slit', 'slitless', 'targacq']
 # nircam: ['coron', 'grism', 'image', 'targacq', 'wfss']
 # niriss: ['ami', 'image', 'soss', 'wfss']
 # nirspec: ['bots', 'ifu', 'msa', 'slit']
@@ -44,26 +56,41 @@
 # Note: with -vv, a list of all filetypes of the observations is shown on screen after the ProductTable
 # is queried for the first time. Example:
 # List of all filetypes of obtained products: ['_segm.fits', '_asn.json', '_pool.csv', '_i2d.jpg', '_thumb.jpg', '_cat.ecsv', '_i2d.fits', '_stream.fits', '_uncal.fits', '_uncal.jpg', '_cal.fits', '_trapsfilled.fits', '_cal.jpg', '_rate.jpg', '_rateints.jpg', '_trapsfilled.jpg', '_rate.fits', '_rateints.fits']
 # If not specified, all products are selected
 #filetypes: ['uncal']
 filetypes: ['fits']
 
-# specify the SCAs.
+# specify the SCAs if querying for NIRCam data.
 # choices=['a1','a2','a3','a4','along','b1','b2','b3','b4','blong']
 # If not specified, all SCAs are selected
+# sca: a1
+# sca: [a1, a3]
 sca:
 
 # if guidestars is set to True, guidestar products are also included
 guidestars: False
 
 # lookback time in days
 # Note that all other time parameters (date_select) override the lookback time.
 lookbacktime: 1.0
 
+# Specify date range (MJD or isot format) applied to "dateobs_center" column. If single value, then exact match.
+# If single value has "+" or "-" at the end, then it is a lower and upper limit, respectively. date_select will
+# override the lookback parameter value.
+# Examples: 58400+, 58400-,2020-11-23+, 2020-11-23 2020-11-25, 59934 59934.125
+# date_select: 2021-05-23+
+# date_select: 2022-06-06 2022-06-08
+date_select:
+
+# save the tables (selected products, obsTable, summary with suffix selprod.txt, obs.txt, summary.txt, respectively) with the
+# specified string as basename. Tables will be saved in outrootdir.
+# If left empty, the tables will not be saved.
+savetables:
+
 # columns returned from MAST to the obsTable
 # The default set in the code is mastcolumns_obsTable=['proposal_id','dataURL','obsid','obs_id','t_min','t_exptime']
 mastcolumns_obsTable: ['proposal_id','dataURL','obsid','obs_id','t_min','t_exptime','instrument_name']
 
 # output columns for the tables. Note that the columns for the individual filetypes
 # are automatically added to the obsTable.
 # The defaults set in the code are:
@@ -91,14 +118,17 @@
 # The defaults set in the code are below, sorting the table in the order the observations were taken:
 # sortcols_summaryTable=['date_start','proposal_id','obsnum']
 # An alternative would be to sort it by propID and obsnum, and not in chronologaical order
 # sortcols_summaryTable: ['proposal_id','obsnum']
 sortcols_summaryTable: ['date_start','proposal_id','obsnum']
 
 #####################################################################################################
+# Create an index.html for each propID that shows thumbnails and metadata of each downloaded product
+makewebpages: False
+
 # specify the product table properties for the webpage
 # first the figure box sizes. recommended: 100-150, or don't specify if webpage_mkthumbnails, since then
 # the size of the thumbnails are used by default.
 webpage_tablefigsize_width:
 webpage_tablefigsize_height:
 
 # list of filetypes for which jpgs should be shown!
@@ -117,20 +147,7 @@
 webpage_mkthumbnails: True
 # redo the thumbnails even if exists if webpage_thumbnails_overwrite is True
 webpage_thumbnails_overwrite: False
 # scale the image down so that it fits the width and height. If only one is specified, then the aspect ratio
 # of the original image is restored
 webpage_thumbnails_width: 120
 webpage_thumbnails_height:
-
-#####################################################################################################
-# The following are other parameters that can be set in the config file, they just need to be uncommented.
-# As a rule, all optional arguments can also be set in the config file. If an optional argument is not None, then it
-# overrides the config file entries
-
-# Specify date range (MJD or isot format) applied to "dateobs_center" column. If single value, then exact match.
-# If single value has "+" or "-" at the end, then it is a lower and upper limit, respectively.
-# Examples: 58400+, 58400-,2020-11-23+, 2020-11-23 2020-11-25
-# date_select: 2021-05-23+
-
-# save the tables (selected products, obsTable, summary with suffix selprod.txt, obs.txt, summary.txt, respectively) with the specified string as basename
-savetables:
```

### Comparing `jwst_mast_query-0.0.2/jwst_mast_query/jwst_query.py` & `jwst_mast_query-0.0.3/jwst_mast_query/jwst_query.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import argparse,os,sys,re,copy,shutil
 import yaml
 from PIL import Image
 
 # pdastroclass is wrapper around pandas.
 from jwst_mast_query.pdastro import pdastroclass,unique,AnotB,AorB,AandB,split_commonpath
 
-from jwst_mast_query.utils.constants import MAST_OBS_MODES
+from jwst_mast_query.utils.constants import MAST_OBS_MODES, PARAM_DEFAULTS
 
 # MAST API documentation:
 # https://mast.stsci.edu/api/v0/pyex.html
 
 # MAST CAOM Field Descriptions:
 # https://mast.stsci.edu/api/v0/_c_a_o_mfields.html
 
@@ -160,131 +160,191 @@
         self.ix_selected_products = None
 
         # indices for obsTable, sorted by self.params['sortcols_obsTable'] (can also be set in config file)
         self.ix_obs_sorted = None
         # indices for summary table, sorted by self.params['sortcols_summaryTable'] (can also be set in config file)
         self.ix_summary_sorted = None
 
-        # columns returned from MAST to the obsTable
-        #self.mastcolumns_obsTable = ['proposal_id','dataURL','obsid','obs_id','t_min','t_exptime']
+        # self.params will be populated from define_options()
+        self.params = deepcopy(PARAM_DEFAULTS)
 
-        # output columns for the tables. Note that the columns for the individual filetypes
-        # are automatically added to the obsTable
-        #self.outcolumns_productTable = ['proposal_id','obsnum','obsID','parent_obsid','obs_id','dataproduct_type','productFilename','filetype','calib_level','size','description']
-        #self.outcolumns_obsTable = ['proposal_id','obsnum','obsid','obs_id','t_min','t_exptime','date_min']
-
-        # self.params will be populated with the arguments
-        self.params = {}
-
-        # columns returned from MAST to the obsTable
-        # These are the default values, they can be changed in the config file
-        self.params['mastcolumns_obsTable']=['proposal_id','dataURL','obsid','obs_id','t_min','t_exptime','instrument_name']
-
-        # output columns for the tables. Note that the columns for the individual filetypes
-        # are automatically added to the obsTable
-        # These are the default values, they can be changed in the config file
-        self.params['outcolumns_productTable']=['proposal_id','obsnum','obsID','parent_obsid','obs_id','sca','visit','dataproduct_type','productFilename','filetype','calib_level','size','description']
-        self.params['outcolumns_obsTable']=['proposal_id','obsnum','obsid','obs_id','t_min','t_exptime','date_min','instrument_name']
-
-        # The productTable is sorted based on these columns  (can also be set in config file)
-        self.params['sortcols_productTable']=['calib_level','filetype','obsID']
-        # The obsTable is sorted based on these columns  (can also be set in config file)
-        self.params['sortcols_obsTable']=['date_min','proposal_id','obsnum']
-        # The summary table is sorted based on these columns (can also be set in config file)
-        self.params['sortcols_summaryTable']=['date_start','proposal_id','obsnum']
-
-        self.params['instrument']='nircam'
-        self.params['filetypes']=['uncal']
-        self.params['guidestars']=False
-        self.params['lookbacktime']=1.0
-
-
-        self.params['skip_propID2outsubdir']=None
-        self.params['obsnum2outsubdir']=None
-        self.params['propIDs_obsnum2outsubdir']=[]
-        self.params['jpg_separate_subdir']=False
-
-        self.params['webpage_tablefigsize_width']=100
-        self.params['webpage_tablefigsize_height']=None
-        self.params['webpage_level12_jpgs']=['_uncal.jpg','_dark.jpg','_rate.jpg','_rateints.jpg','_trapsfilled.jpg','_cal.jpg','_crf.jpg']
-
-
-
-    def define_options(self,parser=None,usage=None,conflict_handler='resolve'):
+    def define_options(self, parser=None, usage=None, conflict_handler='resolve'):
         if parser is None:
-            parser = argparse.ArgumentParser(usage=usage,conflict_handler=conflict_handler)
-
-        # default for config file, if available
-        if 'JWST_QUERY_CFGFILE' in os.environ and os.environ['JWST_QUERY_CFGFILE'] != '':
-            cfgfilename = os.environ['JWST_QUERY_CFGFILE']
-        else:
-            cfgfilename = None
-
-        # default for config file, if available
-        #if 'JWST_QUERY_OUTDIR' in os.environ and os.environ['JWST_QUERY_OUTDIR'] != '':
-        #    defaultoutdir = os.environ['JWST_QUERY_OUTDIR']
-        #else:
-        #    defaultoutdir = None
-
+            parser = argparse.ArgumentParser(usage=usage, conflict_handler=conflict_handler)
 
-        # default for token is $MAST_API_TOKEN
-        if 'MAST_API_TOKEN' in os.environ:
-            defaulttoken = os.environ['MAST_API_TOKEN']
-        else:
-            defaulttoken = None
-
-
-        parser.add_argument('-i', '--instrument', type=str, default=None, choices=['niriss','nircam','nirspec','miri','fgs'], help='Instrument.  (default=%(default)s)')
-        parser.add_argument('--obsmode', type=str, nargs='+', default=None, help='Observing modes. e.g. "imaging, wfss"')
-        parser.add_argument('-v','--verbose', default=0, action='count')
-        parser.add_argument('--propID', type=int, nargs="+", default=None, help='Search for data for this proposal ID(=APT #) only. If more than one argument: all following arguments are a list of obsnum\'s')
-        parser.add_argument('--obsnums', type=int, nargs='+', default=None, help='Search for data in these observation numbers only.')
-        parser.add_argument('--guidestars', action='store_true', default=None, help='Don\'t skip guidestars. By default, they are skipped')
-        parser.add_argument('-f','--filetypes',  type=str, nargs="+", default=None, help=('List of product filetypes to get, e.g., _uncal.fits or _uncal.jpg. If only letters, then _ and .fits are added, for example uncal gets expanded to _uncal.fits. Typical image filetypes are uncal, rate, rateints, cal (default=%(default)s)'))
-        parser.add_argument('--calib_levels',  type=int, nargs="+", default=None, help=('Only select products with the specified calibration levels (calib_level column in productTable) (default=%(default)s)'))
-
-        parser.add_argument('--Nobs_per_batch', type=int, default=None, help='When querying for products for a given list of observations, split into batches of N observations per batch. This helps to prevent time outs when querying for large lists of products!')
-
-        parser.add_argument('-c','--configfile', type=str, default=cfgfilename, help='optional config file. default is set to $JWST_QUERY_CFGFILE. Use -vvv to see the full list of all set parameters.')
-        parser.add_argument('--login', default=None, nargs=2, help='username and password for login')
-        parser.add_argument('--token', type=str, default=defaulttoken, help='MAST API token. You can also set the token in the environment variable \$MAST_API_TOKEN')
-
-        parser.add_argument('--outrootdir', default=None, help='output root directory (default=%(default)s)')
-        parser.add_argument('--outsubdir', default=None, help='outsubdir added to output root directory (default=%(default)s)')
-        parser.add_argument('--skip_propID2outsubdir', action='store_true', default=None, help='By default, the APT proposal ID is added as a subdir to the output directory. You can skip this with this option (default=%(default)s)')
-
-        parser.add_argument('--skip_check_if_outfile_exists', action='store_true', default=None, help='Don\'t check if output files exists. This makes it faster for large lists, but files might be reloaded')
-        parser.add_argument('--skip_check_filesize', action='store_true', default=None, help='Don\'t check if output files have the correct filesize. This makes it faster for large lists, but files might be corrupted.')
-
-        parser.add_argument('-e','--obsid_select', nargs="+", default=[], help='Specify obsid range applied to "obsID" and "parent_obsid" columns in the PRODUCT table. If single value, then exact match. If single value has "+" or "-" at the end, then it is a lower and upper limit, respectively. If two values, then range. Examples: 385539+, 385539-, 385539 385600 (default=%(default)s)')
-        parser.add_argument('-l','--obsid_list', nargs="+", default=[], help='Specify list of obsid applied to "obsID" and "parent_obsid" columns in the PRODUCT table. examples: 385539 385600 385530 (default=%(default)s)')
-#        parser.add_argument('--obnum_list', nargs="+", default=[], help='Specify list of obsnum (default=%(default)s)')
-        parser.add_argument('--sca', nargs="+", default=None, choices=['a1','a2','a3','a4','a5','along','b1','b2','b3','b4','b5','blong','guider1','guider2','nrs1','nrs2','mirimage','mirifulong','mirifushort','nis'], help='Specify list of sca\'s to select. a5=along, b5=blong')
+        parser.add_argument('-i', '--instrument', type=str, default=PARAM_DEFAULTS['instrument'], choices=['niriss','nircam','nirspec','miri','fgs'],
+                            help='Specify the instrument (nircam, nirspec, niriss, miri, fgs)  (default=%(default)s)')
+        parser.add_argument('--obsmode', type=str, nargs='+', default=PARAM_DEFAULTS['obsmode'], help=('Optionally specify the observation modes to query for. '
+                                                                                                       'If provided, MAST will be queried only for these types of '
+                                                                                                       'observations. e.g. assuming instrument is "nircam", '
+                                                                                                       'obsmode: ["image", "wfss"] will query MAST for NIRCAM/IMAGE '
+                                                                                                       'and NIRCAM/WFSS data. If left empty, the query will include '
+                                                                                                       'all modes. For a list of valid modes, see the example config '
+                                                                                                       'file in the repository. Note that as of 24 March 2023, MAST '
+                                                                                                       'is in the process of reprocessing all data to add the mode '
+                                                                                                       'values to the instrument names. Until this process is '
+                                                                                                       'complete, some older data may not include the mode name, '
+                                                                                                       'and therefore will not be found via a query that includes '
+                                                                                                       'the mode name. (default=%(default)s)'))
+        parser.add_argument('-v','--verbose', default=PARAM_DEFAULTS['verbose'], action='count')
+        parser.add_argument('--propID', type=int, nargs="+", default=PARAM_DEFAULTS['propID'], help=('Specify the JWST proposal number to query for. This can be '
+                                                                                                     'a 5 digit integer, or for a smaller number, an integer '
+                                                                                                     'with or without prepended zeros. e.g. 1409 or 01409.'))
+        parser.add_argument('--obsnums', type=int, nargs='+', default=PARAM_DEFAULTS['obsnums'], help=('Specify the observation numbers within the propID. This '
+                                                                                                       'can be a single number, or a bracketed list of numbers. '
+                                                                                                       'e.g. 3 or [3, 103] (default=%(default)s)'))
+        parser.add_argument('--guidestars', action='store_true', default=PARAM_DEFAULTS['guidestars'], help=('If this is set to True, guidestar products are '
+                                                                                                             'also included. Note: there are a **lot** of guide '
+                                                                                                             'star products. We recommend you set to True only if '
+                                                                                                             'really needed! (default=%(default)s)'))
+        parser.add_argument('-f','--filetypes',  type=str, nargs="+", default=PARAM_DEFAULTS['filetypes'], help=('List of file types to select in the product table, '
+                                                                                                                 'e.g., _uncal.fits or _uncal.jpg. If no suffix is '
+                                                                                                                 'given, .fits is appended. If only letters, then _ '
+                                                                                                                 'and .fits are added. For example, "uncal" gets '
+                                                                                                                 'expanded to _uncal.fits. Typical image filetypes '
+                                                                                                                 'are uncal, rate, rateints, cal. For downloading a '
+                                                                                                                 'single file type, the brackets must still surround '
+                                                                                                                 'the file suffix, as the script expects a list. A '
+                                                                                                                 'relatively complete list of options includes: '
+                                                                                                                 '["_segm.fits", "_asn.json", "_pool.csv", "_i2d.jpg", '
+                                                                                                                 '"_thumb.jpg", "_cat.ecsv", "_i2d.fits", "_uncal.fits", '
+                                                                                                                 '"_uncal.jpg", "_cal.fits", "_trapsfilled.fits", '
+                                                                                                                 '"_cal.jpg", "_rate.jpg", "_rateints.jpg", '
+                                                                                                                 '"_trapsfilled.jpg", "_rate.fits", "_rateints.fits"] '
+                                                                                                                 'See the JWST calibration pipeline documentation for '
+                                                                                                                 'a complete list. (default=%(default)s)'))
+        parser.add_argument('--calib_levels',  type=int, nargs="+", default=PARAM_DEFAULTS['calib_levels'], help=('Only select products with the specified '
+                                                                                                                   'calibration levels (calib_level column in '
+                                                                                                                   'productTable) (default=%(default)s)'))
+        parser.add_argument('--Nobs_per_batch', type=int, default=PARAM_DEFAULTS['Nobs_per_batch'], help=('For large programs, the query for the products can time '
+                                                                                                          'out, and in these cases it is better to split up the query '
+                                                                                                          'into Nobs_per_batch observations per batch. For example, '
+                                                                                                          'if there are 22 observations, and Nobs_per_batch=4, then '
+                                                                                                          'there will be 6 batches, 5 batches with 4 observations, '
+                                                                                                          'and the last batch with 2. (default=%(default)s)'))
+        parser.add_argument('-c','--configfile', type=str, default=PARAM_DEFAULTS['configfile'], help=('optional config file. default is set to $JWST_QUERY_CFGFILE. '
+                                                                                                       'Use -vvv to see the full list of all set parameters.'))
+        parser.add_argument('--login', default=PARAM_DEFAULTS['login'], nargs=2, help='username and password for login')
+        parser.add_argument('--token', type=str, default=PARAM_DEFAULTS['token'], help=('MAST API token. You can also set the token in the environment '
+                                                                                        'variable \$MAST_API_TOKEN'))
+        parser.add_argument('--outrootdir', default=PARAM_DEFAULTS['outrootdir'], help=('The base directory for the downloaded products. This can be the name of '
+                                                                                        'an environment variable (such as JWSTDOWNLOAD_OUTDIR), or '
+                                                                                        'a path. Note the preceding "$" in the case where an environment variable is '
+                                                                                        'given. If you include the --outrootdir command line argument when calling '
+                                                                                        'jwst_query.py or jwst_download.py, that value will override any value '
+                                                                                        'provided in the config file. (default=%(default)s)'))
+        parser.add_argument('--outsubdir', default=PARAM_DEFAULTS['outsubdir'], help=('Any additional directory to add to the base directory. This can be used to '
+                                                                                      'customize the organization of the downloaded products. (default=%(default)s)'))
+        parser.add_argument('--obsnum2outsubdir', default=PARAM_DEFAULTS['obsnum2outsubdir'], help=('If True, the observation number will be used to create a '
+                                                                                                    'subdirectory into which the appropriate files will be placed. '
+                                                                                                    'e.g. $JWSTDOWNLOAD_OUTDIR/01410/obsnum23/'))
+        parser.add_argument('--propIDs_obsnum2outsubdir', default=PARAM_DEFAULTS['propIDs_obsnum2outsubdir'], help=('Specify list of propID for which obsnum2outsubdir '
+                                                                                                                    'is True. Only for the listed proposal numbers will '
+                                                                                                                    'observation numbers be used to create a '
+                                                                                                                    'subdirectory into which the appropriate files will '
+                                                                                                                    'be placed. e.g. $JWSTDOWNLOAD_OUTDIR/01410/obsnum23/'))
+        parser.add_argument('--skip_propID2outsubdir', action='store_true', default=PARAM_DEFAULTS['skip_propID2outsubdir'], help=('By default, the APT proposal ID '
+                                                                                                                                   'is added as a subdir to the output '
+                                                                                                                                   'directory. You can skip this with '
+                                                                                                                                   'this option (default=%(default)s)'))
+        parser.add_argument('--skip_check_if_outfile_exists', action='store_true', default=PARAM_DEFAULTS['skip_check_if_outfile_exists'],
+                            help=('By default, the script queries MAST for products, and then checks if each file already exists in the output directory or not '
+                                  '("dl_code" and "dl_str" columns). For large numbers of products, this can take time. By setting this option to True, this '
+                                  'check can be skipped. (default=%(default)s)'))
+        parser.add_argument('--skip_check_filesize', action='store_true', default=PARAM_DEFAULTS['skip_check_filesize'], help=('Don\'t check if output files have the '
+                                                                                                                               'correct filesize. This makes it faster '
+                                                                                                                               'for large lists, but files might be '
+                                                                                                                               'corrupted.'))
+        parser.add_argument('-e','--obsid_select', nargs="+", default=PARAM_DEFAULTS['obsid_select'], help=('Specify obsid range applied to "obsID" and "parent_obsid" '
+                                                                                                            'columns in the PRODUCT table. If single value, then exact '
+                                                                                                            'match. If single value has "+" or "-" at the end, then it '
+                                                                                                            'is a lower and upper limit, respectively. If two values, '
+                                                                                                            'then range. Examples: 385539+, 385539-, 385539 385600 '
+                                                                                                            '(default=%(default)s)'))
+        parser.add_argument('-l','--obsid_list', nargs="+", default=PARAM_DEFAULTS['obsid_list'], help=('Specify list of obsid applied to "obsID" and "parent_obsid" '
+                                                                                                        'columns in the PRODUCT table. examples: 385539 385600 385530 '
+                                                                                                        '(default=%(default)s)'))
+        parser.add_argument('--sca', nargs="+", default=PARAM_DEFAULTS['sca'],
+                            choices=['a1','a2','a3','a4','a5','along','b1','b2','b3','b4','b5','blong',
+                                     'guider1','guider2','nrs1','nrs2','mirimage','mirifulong','mirifushort','nis'],
+                                     help='Specify list of sca\'s to select. a5=along, b5=blong')
+        parser.add_argument('--mastcolumns_obsTable', nargs="+", default=PARAM_DEFAULTS['mastcolumns_obsTable'], help=('Core columns returned from MAST to the obsTable. '
+                                                                                                                       '(default=%(default)s)'))
+        parser.add_argument('--outcolumns_obsTable', nargs="+", default=PARAM_DEFAULTS['outcolumns_obsTable'], help=('Output columns for the obsTable. '
+                                                                                                                     '(default=%(default)s)'))
+        parser.add_argument('--sortcols_obsTable', nargs="+", default=PARAM_DEFAULTS['sortcols_obsTable'], help=('The obsTable is sorted based on these columns. '
+                                                                                                                       'The defaults sort the table in the order the '
+                                                                                                                       'observations were observed. (default=%(default)s)'))
+        parser.add_argument('--outcolumns_productTable', nargs="+", default=PARAM_DEFAULTS['outcolumns_productTable'], help=('List of columns to be shown in product '
+                                                                                                                             'table (default=%(default)s)'))
+        parser.add_argument('--sortcols_productTable', nargs="+", default=PARAM_DEFAULTS['sortcols_productTable'], help=('The productTable is sorted based on these '
+                                                                                                                         'columns. The default sorts the table based '
+                                                                                                                         'on calibration level. (default=%(default)s)'))
+        parser.add_argument('--sortcols_summaryTable', nargs="+", default=PARAM_DEFAULTS['sortcols_summaryTable'], help=('The summary table is sorted based on these '
+                                                                                                                         'columns. The default sorts the table in the '
+                                                                                                                         'order the observations were observed. '
+                                                                                                                         '(default=%(default)s)'))
+        parser.add_argument('--jpg_separate_subdir', default=PARAM_DEFAULTS['jpg_separate_subdir'], help=('If True, downloaded jpgs are saved in separate "jpg" '
+                                                                                                          'subdirectories, along side the fits files. (default=%(default)s)'))
 
         time_group = parser.add_argument_group("Time constraints for the observation/product search")
-
-        time_group.add_argument('-l', '--lookbacktime', type=float, default=None, help='lookback time in days.')
-#        time_group.add_argument('--mjd_min', type=float, default=None, help='minimum MJD. overrides lookback time.')
-#        time_group.add_argument('--mjd_max', type=float, default=None, help='maximum MJD. overrides lookback time.')
-#        time_group.add_argument('-m', '--mjd_limits', default=None, type=float, nargs=2, help='specify the MJD limits. overrides lookback time and mjd_min/max optional arguments.')
-#        time_group.add_argument('-d', '--date_limits', default=None, type=str, nargs=2, help='specify the date limits (ISOT format). overrides lookback time and mjd* optional arguments.')
-        time_group.add_argument('-d','--date_select', nargs="+", default=[], help='Specify date range (MJD or isot format) applied to "dateobs_center" column. If single value, then exact match. If single value has "+" or "-" at the end, then it is a lower and upper limit, respectively. Examples: 58400+, 58400-,2020-11-23+, 2020-11-23 2020-11-25  (default=%(default)s)')
-
-#        time_group.add_argument('--lre3', action='store_true', default=None, help='Use the LRE-3 date limits. Overrides lookback and mjd* options.')
-#        time_group.add_argument('--lre4', action='store_true', default=None, help='Use the LRE-4 date limits. Overrides lookback and mjd* options.')
-#        time_group.add_argument('--lre5', action='store_true', default=None, help='Use the LRE-5 date limits. Overrides lookback and mjd* options.')
-#        time_group.add_argument('--lre6', action='store_true', default=None, help='Use the LRE-6 date limits. Overrides lookback and mjd* options.')
-
-        parser.add_argument('-s', '--savetables', type=str, default=None, help='save the tables (selected products, obsTable, summary with suffix selprod.txt, obs.txt, summary.txt, respectively) with the specified string as basename (default=%(default)s)')
-        parser.add_argument('-w', '--makewebpages', action='store_true', default=False, help='Make webpages for the products for each propID using the downloaded *jpg files')
-
+        time_group.add_argument('-l', '--lookbacktime', type=float, default=PARAM_DEFAULTS['lookbacktime'], help=('Lookback time in days. The script will query MAST '
+                                                                                                                  'over a time from the lookback time to the present '
+                                                                                                                  'moment. Note that all other time parameters '
+                                                                                                                  '(date_select, etc) override the lookback time. '
+                                                                                                                  '(default=%(default)s)'))
+        time_group.add_argument('-d','--date_select', nargs="+", default=PARAM_DEFAULTS['date_select'], help=('Specify date range (MJD or isot format) applied to '
+                                                                                                              '"dateobs_center" column. If single value, then exact '
+                                                                                                              'match. If single value has "+" or "-" at the end, then '
+                                                                                                              'it is a lower and upper limit, respectively. date_select '
+                                                                                                              'will override the lookbacktime. Examples: '
+                                                                                                              '58400+, 58400-,2020-11-23+, 2020-11-23 2020-11-25  '
+                                                                                                              '(default=%(default)s)'))
+        parser.add_argument('-s', '--savetables', type=str, default=PARAM_DEFAULTS['savetables'], help=('Save the tables (selected products, obsTable, summary with '
+                                                                                                        'suffix selprod.txt, obs.txt, summary.txt, respectively) with '
+                                                                                                        'the specified string as basename. Tables are saved in the '
+                                                                                                        'same output directory as the data.  If no string is '
+                                                                                                        'provided, the tables are not saved. (default=%(default)s)'))
+        parser.add_argument('-w', '--makewebpages', action='store_true', default=PARAM_DEFAULTS['makewebpages'],
+                            help=('Make webpages for the products for each propID containing info and images of the retrieved data. Note that this option is not '
+                                  'currently in the config file, and must be specified at the command line. (default=%(default)s)'))
+        parser.add_argument('--webpage_tablefigsize_width', default=PARAM_DEFAULTS['webpage_tablefigsize_width'], help=("Width in pixels of the resized jpg images "
+                                                                                                                        "to be inserted into the index.html summary file."
+                                                                                                                        "Recommended: 100-150, or don't specify if "
+                                                                                                                        "webpage_mkthumbnails, since then the size of "
+                                                                                                                        "the thumbnails are used by default. "
+                                                                                                                        "(default=%(default)s)"))
+        parser.add_argument('--webpage_tablefigsize_height', default=PARAM_DEFAULTS['webpage_tablefigsize_height'], help=("Height in pixels of the resized jpg images "
+                                                                                                                          "to be inserted into the index.html summary "
+                                                                                                                          "file. If left undefined, the height will be "
+                                                                                                                          "determined from webpage_thumbnail_width and "
+                                                                                                                          "the aspect ratio of the original image.  "
+                                                                                                                          "(default=%(default)s)"))
+        parser.add_argument('--webpage_level12_jpgs', nargs="+", default=PARAM_DEFAULTS['webpage_level12_jpgs'], help=('List of filetypes whose thumbnails will be shown in '
+                                                                                                            'index.html. (default=%(default)s)'))
+        parser.add_argument('--webpage_fitskeys2table', nargs="+", default=PARAM_DEFAULTS['webpage_fitskeys2table'], help=('List of fits header keywords that should '
+                                                                                                                           'be copied to the table. (default=%(default)s)') )
+        parser.add_argument('--webpage_cols4table', nargs="+", default=PARAM_DEFAULTS['webpage_cols4table'], help=('Columns to be shown in index.html. (default=%(default)s)'))
+        parser.add_argument('--webpage_sortcols', nargs="+", default=PARAM_DEFAULTS['webpage_sortcols'], help=('Columns to sort index.html by. (default=%(default)s)'))
+        parser.add_argument('--webpage_mkthumbnails', default=PARAM_DEFAULTS['webpage_mkthumbnails'], help=('If True, a thumbnail jpg is created for each of the '
+                                                                                                            'jpg products listed in webpage_level12_jpgs. '
+                                                                                                            '(default=%(default)s)'))
+        parser.add_argument('--webpage_thumbnails_overwrite', default=PARAM_DEFAULTS['webpage_thumbnails_overwrite'], help=('If True, remake thumbnails even if they '
+                                                                                                                            'already exist (default=%(default)s)'))
+        parser.add_argument('--webpage_thumbnails_width', default=PARAM_DEFAULTS['webpage_thumbnails_width'], help=('Width in pixels of the resized jpg images '
+                                                                                                                    'to be inserted into the index.html summary '
+                                                                                                                    'file. (default=%(default)s)'))
+        parser.add_argument('--webpage_thumbnails_height', default=PARAM_DEFAULTS['webpage_thumbnails_height'], help=('Height in pixels of the resized jpg images '
+                                                                                                                      'to be inserted into the index.html summary '
+                                                                                                                      'file. (default=%(default)s)'))
+        parser.add_argument('--skipdownload', action='store_true', default=PARAM_DEFAULTS['skipdownload'], help='If set, no files will be downloaded. (default=%(default)s)')
 
         return(parser)
 
-    def get_arguments(self, args, configfile = None):
+    def get_arguments(self, args, configfile=None):
         '''
 
         Parameters
         ----------
         args : list
             pass the command line arguments to self.params.
             makes sure that the propID has the correct format (5 digit string)
@@ -316,62 +376,66 @@
                                     raise RuntimeError("environment variable %s used in config file, but not set!" % name)
                             else:
                                 envval=os.environ[name]
                                 subpattern='\$%s' % (name)
                                 paramsdict[param] = re.sub(subpattern,envval,paramsdict[param])
                 elif isinstance(paramsdict[param], dict):
                 #elif type(dict[param]) is types.DictType:
-                    # recursive: sub environment variables down the dictiionary
+                    # recursive: sub environment variables down the dictionary
                     subenvvarplaceholder(paramsdict[param])
             return(0)
 
-
         # get the parameters from the config file
         if args.configfile is not None:
-            #cfgparams = yaml.load_file(args.configfile)
             if not os.path.isfile(args.configfile):
                 raise RuntimeError('config file %s does not exist!' % (args.configfile))
             print(f'Loading config file {args.configfile}')
             cfgparams = yaml.load(open(args.configfile,'r'), Loader=yaml.FullLoader)
             self.params.update(cfgparams)
+            self.params['configfile'] = args.configfile
 
-            # If obsmode is None, change to an empty list
-            if self.params['obsmode'] is None:
-                self.params['obsmode'] = []
+            if args.verbose>2:
+                print('\n### CONFIG FILE PARAMETERS:')
+                for p in cfgparams:
+                    print('config file args: setting %s to' % (p),cfgparams[p])
 
             # Make sure propID and obsnums, if they have been entered in the config file,
-            # are lists, rather than integers.
-            list_keys = ['propID', 'obsnums', 'obsmode']
+            # are lists, rather than integers. When entered via command line, they are
+            # guaranteed to be lists.
+            list_keys = ['propID', 'obsnums']
             for key in list_keys:
                 if key in self.params.keys():
-                    if not isinstance(self.params[key], list):
+                    if not isinstance(self.params[key], list) and self.params[key] is not None:
                         self.params[key] = [self.params[key]]
 
             # Ensure that the propID is a 5-digit string
             if 'propID' in self.params.keys():
-                self.params['propID'] = ['%05d' % (int(self.params['propID'][0]))]
+                if self.params['propID'] is not None:
+                    self.params['propID'] = ['%05d' % (int(self.params['propID'][0]))]
 
-            subenvvarplaceholder(self.params)
+        subenvvarplaceholder(self.params)
 
-            if args.verbose>2:
-                print('\n### CONFIG FILE PARAMETERS:')
-                for p in cfgparams:
-                    print('config file args: setting %s to' % (p),cfgparams[p])
+        # Make sure obsmode is a list, even if it's just [None]
+        list_keys = ['obsmode']
+        for key in list_keys:
+            if key in self.params.keys():
+                if not isinstance(self.params[key], list):
+                    self.params[key] = [self.params[key]]
 
         # Go through optional parameters.
         # 'None' does not overwrite previously set parameters (either default or config file)
         if args.verbose>2:
             print('\n### OPTIONAL COMMAND LINE PARAMETERS:')
         argsdict = vars(args)
         for arg in argsdict:
 
             # skip config file
             if arg=='configfile': continue
 
-            if argsdict[arg] is not None:
+            if argsdict[arg] is not None and argsdict[arg] != []:
                 if args.verbose>2:
                     print('optional args: setting %s to %s' % (arg,argsdict[arg]))
                 self.params[arg]=argsdict[arg]
             else:
                 if arg not in  self.params:
                     self.params[arg]=None
 
@@ -384,15 +448,15 @@
                 self.params['obsnums'] = self.params['propID'][1:]
             self.params['propID'] = '%05d' % (int(self.params['propID'][0]))
         self.verbose = self.params['verbose']
 
         if self.verbose>2:
             print('\n### FINAL PARAMETERS:')
             for p in self.params:
-                print(p,self.params[p])
+                print(f'{p}: {self.params[p]}')
 
         print('INSTRUMENT: ', self.params['instrument'])
         print('obsmode: ', self.params['obsmode'])
         print('propID: ',self.params['propID'])
         print('obsnums: ',self.params['obsnums'])
 
         return(0)
@@ -530,14 +594,20 @@
         mjd_max : float
             MJD of the latest time to search
         """
         if lookbacktime is None: lookbacktime = self.params['lookbacktime']
 
         if date_select is None: date_select = self.params['date_select']
 
+        # If date_select is a string, split it into a list.
+        # When provided at the command line, date_select is a list.
+        # When provided in cfg file, date_select is a string.
+        if isinstance(date_select, str):
+            date_select = date_select.split(' ')
+
         mjd_min = mjd_max = None
         # parse trailing '+' and '-', and get limits
         limits = getlimits(date_select)
         if limits is not None:
             # Convert dates into MJD if necessary
             for i in (0,1):
                 if limits[i] is not None:
@@ -593,15 +663,16 @@
 
         # To get the list of modes, we can query using Observations, which does support
         # wildcard characters, but returnes only limited information. In this case, we
         # care only about the instrument_name values in the results.
 
         # Check to see if the user entered a list of observing modes. If not, we
         # query all modes for the instrument via wildcard
-        if len(self.params['obsmode']) == 0:
+        if self.params['obsmode'][0] is None or len(self.params['obsmode']) == 0:
+            print(f'No obsmode given. Querying for all files for {instrument}.')
             inst_list = list(set(Observations.query_criteria(instrument_name=f'{instrument}*',
                                                              t_min=[mjd_min, mjd_max])['instrument_name']))
         else:
             initial_inst_list = [f'{instrument.upper()}/{mode.upper()}' for mode in self.params['obsmode']]
             inst_list = deepcopy(initial_inst_list)
 
             # Check against the set of allowed modes, and alert the user to any invalid entries
@@ -618,14 +689,18 @@
 
             # If all of the user-input obsmodes are invalid, then we fall back to using the wildcard
             if len(inst_list) == 0:
                 print('All entered modes are invalid. Falling back to query across all possible obsmodes.')
                 inst_list = list(set(Observations.query_criteria(instrument_name=f'{instrument}*',
                                                              t_min=[mjd_min, mjd_max])['instrument_name']))
 
+        # If inst_list is empty, then there are no observations to query for
+        if len(inst_list) == 0:
+            return(0)
+
         columns = ','.join(self.params['mastcolumns_obsTable'])
         service = self.SERVICES['Caom_search']
         params = {"columns":columns,
                   "filters":[
                   {"paramName":"obs_collection","values":["JWST"]},
                   {"paramName":"instrument_name","values":inst_list},
                   {"paramName":"t_min",
@@ -862,18 +937,26 @@
                 if self.verbose:
                     print(f'Querying products for obsids={obsids}')
                 params = {"obsid":obsids,
                           "columns":['type','productType'],
                           "format":"json"
                           }
                 tmptable = self.JwstObs.service_request(service, params).to_pandas()
+
+                # Remove duplicate rows based on the productFilename value
+                tmptable.drop_duplicates(subset='productFilename', keep='first', inplace=True, ignore_index=True)
+
                 if self.verbose:
-                    print(f'{len(tmptable)} products found for this chunk of observations')
+                    print(f'After filtering duplicate entries, {len(tmptable)} products found for this chunk of observations')
                 tmptables.append(tmptable)
+
             self.productTable.t = pd.concat(tmptables, axis=0, ignore_index=True)
+
+            # Remove duplicate rows that come from different queries
+            self.productTable.t.drop_duplicates(subset='productFilename', keep='first', inplace=True, ignore_index=True)
         else:
             params = {"obsid":obsids,
                       "columns":['type','productType'],
                       "format":"json"
                       }
             if self.verbose:
                 print('\n#### Querying ProductTable....')
@@ -1130,15 +1213,14 @@
         self.outrootdir = outrootdir
         if self.outrootdir is None:
             self.outrootdir = self.params['outrootdir']
         # if outdir is not defined, use '.'
         if self.outrootdir is None or self.outrootdir == '':
             self.outrootdir = '.'
 
-
         if outsubdir is not None and outsubdir!='':
             self.outrootdir  += f'/{outsubdir}'
         elif self.params['outsubdir'] is not None and self.params['outsubdir']!='':
             self.outrootdir  += f'/{self.params["outsubdir"]}'
 
         self.outrootdir = os.path.abspath(self.outrootdir)
         return(self.outrootdir)
@@ -1451,34 +1533,40 @@
 
                 # make a thumbnail that links to the full size image
                 productTable.t.loc[ix,figcol]=image4table(jpgname,TNimagename=TNjpgname,width=width,height=height)
                 #productTable.t.loc[ix,figcol]=addlink2string(imagestring4web(jpgname,width=None,height=p),jpgname)
 
         outcols4html = self.params['webpage_cols4table']
 
-        # make the ascci table(without the jpg cols), and save it
+        # Make the ascci table(without the jpg cols), and save it.
+        # Use a try/except to insulate against the case where requested suffixes for download in webpage_level12_jpgs
+        # are not included in webpage_cols4table
         outcols4ascci = copy.deepcopy(outcols4html)
         for figcol in figcols:
-            outcols4ascci.remove(figcol)
-        print(f'writing {description} pandas ascii to {asciiname}')
+            try:
+                outcols4ascci.remove(figcol)
+            except ValueError:
+                pass
+        print(f'Writing {description} pandas ascii to {asciiname}')
+        print(outcols4ascci)
         productTable.write(filename=asciiname, indices=ixs_uncal, columns=outcols4ascci)
 
         # write the table to index.html
         print(f'writing {description} html to {htmlname}')
         f=open(htmlname,'w')
         s_asciilink = addlink2string('ascii-table',os.path.basename(asciiname))
         f.writelines([f'Level 1+2 Products for {description} ({s_asciilink} here)'])
         (errorflag,lines)=productTable.write(return_lines=True, indices=ixs_uncal, columns=outcols4html, htmlflag=True, htmlsortedtable=True, escape=False)
         if errorflag: raise RuntimeError(f'Soemthing went wrong when doing the webpage table for {description}')
         f.writelines(lines)
         f.close()
 
         # Make sure sortable.js is in the html directory
         htmldir = os.path.dirname(htmlname)
-        jsfilename = f'{os.path.dirname(os.path.realpath(sys.argv[0]))}/sortable.js'
+        jsfilename = os.path.join(os.path.realpath(os.path.dirname(os.path.join('../', __file__))), 'sortable.js')
         dest_jsfilename = f'{htmldir}/sortable.js'
         if not os.path.isfile(dest_jsfilename):
             if not os.path.isfile(jsfilename):
                 raise RuntimeError(f'java script {jsfilename} for sortable tables does not exist!')
             shutil.copy(jsfilename, dest_jsfilename)
 
         return(0)
@@ -1517,36 +1605,34 @@
 
 
     def mk_all_tables(self, filetypes=None, showtables=True):
 
         if filetypes is not None:
             self.params['filetypes'] = filetypes
 
-        # get the MJD limits, based on --mjdlimits --lockbacktime --mjdmin --mjdmax --lre3 --lre4 --lre5 --lre6
+        # get the MJD limits, based on --mjdlimits --lockbacktime --mjdmin --mjdmax
         mjd_min, mjd_max = self.get_mjd_limits()
 
         # get the observations: stored in self.obsTable
         self.observation_query(propID=self.params['propID'], mjd_min = mjd_min, mjd_max = mjd_max)
 
         if len(self.obsTable.t)==0:
             print('\n################################\nNO OBSERVATIONS FOUND! exiting....\n################################')
             self.ix_selected_products = []
             return(0)
 
         if self.verbose>1:
             print(self.obsTable.t)
 
-
         # get the products:  stored in self.productTable
         # this list contains in general several entries for each observations.
         # If not otherwise specified, uses self.obsTable as starting point
         self.product_query(Nobs_per_batch=self.params['Nobs_per_batch'])
         if self.verbose>1:
             print(self.productTable.t)
-            #print(self.productTable.columns)
 
         # select the products to download
         # If not otherwise specified, uses self.productTable as starting point
         # uses self.filetypes for filtering, which is set by optional parameters.
         # the selected products indices are put into self.ix_selected_products
         self.product_filter()
 
@@ -1559,43 +1645,47 @@
 
         # get selected SCAs if specified
         self.ix_selected_products = self.select_sca(self.params['sca'])
 
         # only keep entries in the obstable that are parent_obsid in product table
         self.ix_obs_sorted = self.update_obstable_indices(self.ix_selected_products)
 
-        # definte the output filenames, and check if they exist.
+        # define the output filenames, and check if they exist.
         self.mk_outfilenames(skip_propID2outsubdir=self.params['skip_propID2outsubdir'],
                              obsnum2outsubdir=self.params['obsnum2outsubdir'],
                              jpg_separate_subdir=self.params['jpg_separate_subdir'],
                              skip_check_if_outfile_exists=self.params['skip_check_if_outfile_exists'],
                              skip_check_filesize=self.params['skip_check_filesize'])
 
         # update obsTable with selected products: count the different filetypes, and also update the obsnum if None in obsTable
         self.update_obsTable_with_selectedProducts()
 
         # print the table to screen if either verbose or not downloading
         if showtables:
             print('\n######################\n### Selected Products:\n######################')
-            self.productTable.write(indices=self.ix_selected_products,columns=self.params['outcolumns_productTable'])
+            self.productTable.write(indices=self.ix_selected_products, columns=self.params['outcolumns_productTable'])
 
             print('\n#################\n### Observations:\n#################')
             self.obsTable.write(columns=self.params['outcolumns_obsTable'],indices=self.ix_obs_sorted)
 
         # make summary table
         self.mk_summary_tables()
         if showtables:
             print('\n##########################\n### Summary propID/obsnum:\n##########################')
             self.summary.write(indices=self.ix_summary_sorted)
 
         # save the tables if wanted
         if self.params['savetables'] is not None:
-            self.productTable.write(filename=self.params['savetables']+'.selprod.txt',indices=self.ix_selected_products,columns=self.params['outcolumns_productTable'],verbose=2)
-            self.obsTable.write(filename=self.params['savetables']+'.obs.txt',columns=self.params['outcolumns_obsTable'],indices=self.ix_obs_sorted,verbose=2)
-            self.summary.write(filename=self.params['savetables']+'.summary.txt',indices=self.ix_summary_sorted,verbose=2)
+            prodfile = os.path.join(self.outrootdir, self.params['savetables']+'.selprod.txt')
+            obsfile = os.path.join(self.outrootdir, self.params['savetables']+'.obs.txt')
+            summaryfile = os.path.join(self.outrootdir, self.params['savetables']+'.summary.txt')
+
+            self.productTable.write(filename=prodfile, indices=self.ix_selected_products, columns=self.params['outcolumns_productTable'], verbose=2)
+            self.obsTable.write(filename=obsfile, columns=self.params['outcolumns_obsTable'], indices=self.ix_obs_sorted, verbose=2)
+            self.summary.write(filename=summaryfile, indices=self.ix_summary_sorted, verbose=2)
 
         return(0)
 
 
 
 if __name__ == '__main__':
```

### Comparing `jwst_mast_query-0.0.2/jwst_mast_query/pdastro.py` & `jwst_mast_query-0.0.3/jwst_mast_query/pdastro.py`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.2/jwst_mast_query/scripts/jwst_download.py` & `jwst_mast_query-0.0.3/jwst_mast_query/scripts/jwst_download.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     download = jdl.download_mast()
     parser = download.define_options()
     args = parser.parse_args()
 
     # The config file is loaded into self.params, and overwritten with the arguments that are not None
     download.get_arguments(args)
     if download.verbose>2:
-        print('params:', download.params)
+        print('params:')
+        for key, value in download.params.items():
+            print(key, value)
 
     # Use arguments or $API_MAST_TOKEN to login
     download.login(raiseErrorFlag=True)
 
     # self.outrootdir is set depending on outrootdir and outsubdir in cfg file or through the options --outrootdir and --outsubdir
     download.set_outrootdir()
     if download.verbose: print(f'Outdir: {download.outrootdir}')
```

### Comparing `jwst_mast_query-0.0.2/jwst_mast_query/sortable.js` & `jwst_mast_query-0.0.3/jwst_mast_query/sortable.js`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.2/jwst_mast_query.egg-info/PKG-INFO` & `jwst_mast_query-0.0.3/jwst_mast_query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwst-mast-query
-Version: 0.0.2
+Version: 0.0.3
 Summary: Query MAST for JWST products, and download them
 Home-page: https://github.com/spacetelescope/jwst_mast_query
 Author: STScI (Rest)
 Author-email: arest@stsci.edu
 License: UNKNOWN
 Keywords: astronomy
 Platform: UNKNOWN
```

### Comparing `jwst_mast_query-0.0.2/jwst_mast_query.egg-info/SOURCES.txt` & `jwst_mast_query-0.0.3/jwst_mast_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.2/setup.py` & `jwst_mast_query-0.0.3/setup.py`

 * *Files identical despite different names*

