# Comparing `tmp/earthaccess-0.5.1.tar.gz` & `tmp/earthaccess-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthaccess-0.5.1.tar", max compression
+gzip compressed data, was "earthaccess-0.5.2.tar", max compression
```

## Comparing `earthaccess-0.5.1.tar` & `earthaccess-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2023-03-20 14:35:24.203648 earthaccess-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     7972 2023-03-20 14:35:24.203648 earthaccess-0.5.1/README.md
--rw-r--r--   0        0        0      810 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/__init__.py
--rw-r--r--   0        0        0     9627 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/api.py
--rw-r--r--   0        0        0    13493 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/auth.py
--rw-r--r--   0        0        0   207752 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/css/iso_bootstrap4.0.0min.css
--rw-r--r--   0        0        0      199 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/css/styles.css
--rw-r--r--   0        0        0     5495 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/daac.py
--rw-r--r--   0        0        0     1777 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/formatters.py
--rw-r--r--   0        0        0    10706 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/results.py
--rw-r--r--   0        0        0    25069 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/search.py
--rw-r--r--   0        0        0    21685 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/store.py
--rw-r--r--   0        0        0      140 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/utils/_validation.py
--rw-r--r--   0        0        0        0 2023-03-20 14:35:24.203648 earthaccess-0.5.1/earthaccess/widgets.py
--rw-r--r--   0        0        0     1954 2023-03-20 14:35:24.207648 earthaccess-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     9495 1970-01-01 00:00:00.000000 earthaccess-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 00:03:02.080972 earthaccess-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     7873 2023-04-21 00:03:02.080972 earthaccess-0.5.2/README.md
+-rw-r--r--   0        0        0      810 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/__init__.py
+-rw-r--r--   0        0        0     9745 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/api.py
+-rw-r--r--   0        0        0    14106 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/auth.py
+-rw-r--r--   0        0        0   207752 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/css/iso_bootstrap4.0.0min.css
+-rw-r--r--   0        0        0      199 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/css/styles.css
+-rw-r--r--   0        0        0     5495 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/daac.py
+-rw-r--r--   0        0        0     1780 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/formatters.py
+-rw-r--r--   0        0        0    10661 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/results.py
+-rw-r--r--   0        0        0    24980 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/search.py
+-rw-r--r--   0        0        0    21685 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/store.py
+-rw-r--r--   0        0        0      140 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/utils/_validation.py
+-rw-r--r--   0        0        0        0 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/widgets.py
+-rw-r--r--   0        0        0     1918 2023-04-21 00:03:02.088971 earthaccess-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9348 1970-01-01 00:00:00.000000 earthaccess-0.5.2/PKG-INFO
```

### Comparing `earthaccess-0.5.1/LICENSE.txt` & `earthaccess-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.1/README.md` & `earthaccess-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     <img src="https://img.shields.io/pypi/v/earthaccess?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/earthdata/" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/earthaccess.svg" alt="Python Versions">
 </a>
 
-<a href="https://nsidc.github.io/earthdata/" target="_blank">
-    <img src="https://readthedocs.org/projects/earthaccess/badge/?version=latest&style=plastic" alt="Documentation link">
+<a href='https://earthdata.readthedocs.io/en/latest/?badge=latest'>
+    <img src='https://readthedocs.org/projects/earthdata/badge/?version=latest' alt='Documentation Status' />
 </a>
 
 </p>
 
 ## **Overview**
 
 *earthaccess* is a **python library to search, download or stream NASA Earth science data** with just a few lines of code.
@@ -43,15 +43,15 @@
 
 Using Pip
 
 ```bash
 pip install earthaccess
 ```
 
-Try it in your browser without installing anything! [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nsidc/earthdata/main)
+Try it in your browser without installing anything! [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nsidc/earthaccess/main)
 
 
 ## **Usage**
 
 
 With *earthaccess* we can login, search and download data with a few lines of code and even more relevant, our code will work the same way if we are running it in the cloud or from our laptop. ***earthaccess*** handles authentication with [NASA's Earthdata Login (EDL)](https://urs.earthdata.nasa.gov), search using NASA's [CMR](https://cmr.earthdata.nasa.gov/search/site/docs/search/api.html) and access through [`fsspec`](https://github.com/fsspec/filesystem_spec).
 
@@ -70,17 +70,16 @@
     * if available you can use environment variables **EARTHDATA_USERNAME** and **EARTHDATA_PASSWORD**
 3. Interactively entering your EDL credentials
     * You can be prompted for these credentials and save them to a `.netrc` file
 
 ```python
 import earthaccess
 
-auth = earthaccess.login(strategy="netrc")
-if not auth:
-    auth = earthaccess.login(strategy="interactive", persist=True)
+auth = earthaccess.login()
+
 ```
 
 Once you are authenticated with NASA EDL you can:
 
 * Get a file from a DAAC using a `fsspec` session.
 * Request temporary S3 credentials from a particular DAAC (needed to download or stream data from an S3 bucket in the cloud).
 * Use the library to download or stream data directly from S3.
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 [earthaccess, a python library to search, download or stream NASA Earth science
                       data with just a few lines of code]
       [Art_Designer:_Allison_Horst] [Package_version] [Python_Versions]
-                             [Documentation_link]
+                            [Documentation_Status]
 ## **Overview** *earthaccess* is a **python library to search, download or
 stream NASA Earth science data** with just a few lines of code. In the age of
 cloud computing, the power of open science only reaches its full potential if
 we have easy-to-use workflows that facilitate research in an inclusive,
 efficient and reproducible way. Unfortunately âas it stands todayâ
 scientists and students alike face a steep learning curve adapting to systems
 that have grown too complex and end up spending more time on the technicalities
@@ -18,75 +18,74 @@
 systems. Therefore, providing easy access to NASA Earthdata regardless of the
 data storage location (hosted within or outside of the cloud) is the main
 motivation behind this Python library. ## **Installing earthaccess** You will
 need Python 3.8 or higher installed. Install the latest release using conda
 ```bash conda install -c conda-forge earthaccess ``` Using Pip ```bash pip
 install earthaccess ``` Try it in your browser without installing anything! [!
 [Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
-nsidc/earthdata/main) ## **Usage** With *earthaccess* we can login, search and
-download data with a few lines of code and even more relevant, our code will
-work the same way if we are running it in the cloud or from our laptop.
+nsidc/earthaccess/main) ## **Usage** With *earthaccess* we can login, search
+and download data with a few lines of code and even more relevant, our code
+will work the same way if we are running it in the cloud or from our laptop.
 ***earthaccess*** handles authentication with [NASA's Earthdata Login (EDL)]
 (https://urs.earthdata.nasa.gov), search using NASA's [CMR](https://
 cmr.earthdata.nasa.gov/search/site/docs/search/api.html) and access through
 [`fsspec`](https://github.com/fsspec/filesystem_spec). The only requirement to
 use this library is to open a free account with NASA [EDL](https://
 urs.earthdata.nasa.gov). [https://auth.ops.maap-project.org/cas/images/urs-
 logo.png] ### **Authentication** Once you have an EDL account, you can
 authenticate using one of the following three methods: 1. Using a `.netrc` file
 * Can use *earthaccess* to read your EDL credentials (username and password)
 from a `.netrc` file 2. Reading your EDL credentials from environment variables
 * if available you can use environment variables **EARTHDATA_USERNAME** and
 **EARTHDATA_PASSWORD** 3. Interactively entering your EDL credentials * You can
 be prompted for these credentials and save them to a `.netrc` file ```python
-import earthaccess auth = earthaccess.login(strategy="netrc") if not auth: auth
-= earthaccess.login(strategy="interactive", persist=True) ``` Once you are
-authenticated with NASA EDL you can: * Get a file from a DAAC using a `fsspec`
-session. * Request temporary S3 credentials from a particular DAAC (needed to
-download or stream data from an S3 bucket in the cloud). * Use the library to
-download or stream data directly from S3. * Regenerate CMR tokens (used for
-restricted datasets) ### **Searching for data** Once we have selected our
-dataset we can search for the data granules using *doi*, *short_name* or
-*concept_id*. If we are not sure or we don't know how to search for a
-particular dataset, we can start with the ["Introducing NASA earthaccess"]
-(https://nsidc.github.io/earthaccess/tutorials/demo/#querying-for-datasets)
-tutorial or through the [NASA Earthdata Search portal](https://
-search.earthdata.nasa.gov/). For a complete list of search parameters we can
-use visit the extended [API documentation](https://nsidc.github.io/earthaccess/
-user-reference/api/api/). ```python results = earthaccess.search_data
-( short_name='ATL06', version="005", cloud_hosted=True, bounding_box=(-10, 20,
-10, 50), temporal=("2020-02", "2020-03"), count=100 ) ``` Now that we have our
-results we can do multiple things: We can iterate over them to get HTTP (or S3)
-links, we can download the files to a local folder, or we can open these files
-and stream their content directly to other libraries e.g. xarray. ###
-**Accessing the data** **Option 1: Using the data links** If we already have a
-workflow in place for downloading our data, we can use *earthaccess* as a
-search-only library and get HTTP links from our query results. This could be
-the case if our current workflow uses a different language and we only need the
-links as input. ```python # if the data set is cloud hosted there will be S3
-links available. The access parameter accepts "direct" or "external", direct
-access is only possible if you are in the us-west-2 region in the cloud.
-data_links = [granule.data_links(access="direct") for granule in results] # or
-if the data is an on-prem dataset data_links = [granule.data_links
-(access="external") for granule in results] ``` > Note: *earthaccess* can get
-S3 credentials for us, or auhenticated HTTP sessions in case we want to use
-them with a different library. **Option 2: Download data to a local folder**
-This option is practical if you have the necessary space available on disk. The
-*earthaccess* library will print out the approximate size of the download and
-its progress. ```python files = earthaccess.download(results, "./local_folder")
-``` **Option 3: Direct S3 Access - Stream data directly to xarray** This method
-works best if you are in the same Amazon Web Services (AWS) region as the data
-(us-west-2) and you are working with gridded datasets (processing level 3 and
-above). ```python import xarray as xr ds = xr.open_mfdataset(earthaccess.open
-(results)) ``` And that's it! Just one line of code, and this same piece of
-code will also work for data that are not hosted in the cloud, i.e. located at
-NASA storage centers. > More examples coming soon! ### Compatibility Only
-**Python 3.8+** is supported. ## Contributors [![Contributors](https://
-contrib.rocks/image?repo=nsidc/earthaccess)](https://github.com/nsidc/
-earthaccess/graphs/contributors) ## Contributing Guide Welcome! ðð >
-Please see the [Contributing Guide](CONTRIBUTING.md). ### [Project Board]
-(https://github.com/nsidc/earthdata/discussions). ### Glossary NASA_Earth
-Science_Glossary ## License earthaccess is licensed under the MIT license. See
-[LICENSE](LICENSE.txt). ## Level of Support
+import earthaccess auth = earthaccess.login() ``` Once you are authenticated
+with NASA EDL you can: * Get a file from a DAAC using a `fsspec` session. *
+Request temporary S3 credentials from a particular DAAC (needed to download or
+stream data from an S3 bucket in the cloud). * Use the library to download or
+stream data directly from S3. * Regenerate CMR tokens (used for restricted
+datasets) ### **Searching for data** Once we have selected our dataset we can
+search for the data granules using *doi*, *short_name* or *concept_id*. If we
+are not sure or we don't know how to search for a particular dataset, we can
+start with the ["Introducing NASA earthaccess"](https://nsidc.github.io/
+earthaccess/tutorials/demo/#querying-for-datasets) tutorial or through the
+[NASA Earthdata Search portal](https://search.earthdata.nasa.gov/). For a
+complete list of search parameters we can use visit the extended [API
+documentation](https://nsidc.github.io/earthaccess/user-reference/api/api/).
+```python results = earthaccess.search_data( short_name='ATL06', version="005",
+cloud_hosted=True, bounding_box=(-10, 20, 10, 50), temporal=("2020-02", "2020-
+03"), count=100 ) ``` Now that we have our results we can do multiple things:
+We can iterate over them to get HTTP (or S3) links, we can download the files
+to a local folder, or we can open these files and stream their content directly
+to other libraries e.g. xarray. ### **Accessing the data** **Option 1: Using
+the data links** If we already have a workflow in place for downloading our
+data, we can use *earthaccess* as a search-only library and get HTTP links from
+our query results. This could be the case if our current workflow uses a
+different language and we only need the links as input. ```python # if the data
+set is cloud hosted there will be S3 links available. The access parameter
+accepts "direct" or "external", direct access is only possible if you are in
+the us-west-2 region in the cloud. data_links = [granule.data_links
+(access="direct") for granule in results] # or if the data is an on-prem
+dataset data_links = [granule.data_links(access="external") for granule in
+results] ``` > Note: *earthaccess* can get S3 credentials for us, or
+auhenticated HTTP sessions in case we want to use them with a different
+library. **Option 2: Download data to a local folder** This option is practical
+if you have the necessary space available on disk. The *earthaccess* library
+will print out the approximate size of the download and its progress. ```python
+files = earthaccess.download(results, "./local_folder") ``` **Option 3: Direct
+S3 Access - Stream data directly to xarray** This method works best if you are
+in the same Amazon Web Services (AWS) region as the data (us-west-2) and you
+are working with gridded datasets (processing level 3 and above). ```python
+import xarray as xr ds = xr.open_mfdataset(earthaccess.open(results)) ``` And
+that's it! Just one line of code, and this same piece of code will also work
+for data that are not hosted in the cloud, i.e. located at NASA storage
+centers. > More examples coming soon! ### Compatibility Only **Python 3.8+** is
+supported. ## Contributors [![Contributors](https://contrib.rocks/
+image?repo=nsidc/earthaccess)](https://github.com/nsidc/earthaccess/graphs/
+contributors) ## Contributing Guide Welcome! ðð > Please see the
+[Contributing Guide](CONTRIBUTING.md). ### [Project Board](https://github.com/
+nsidc/earthdata/discussions). ### Glossary NASA_Earth_Science_Glossary ##
+License earthaccess is licensed under the MIT license. See [LICENSE]
+(LICENSE.txt). ## Level of Support
 [https://raw.githubusercontent.com/nsidc/earthdata/main/docs/nsidc-logo.png]
 This repository is not actively supported by NSIDC but we welcome issue
 submissions and pull requests in order to foster community contribution.
```

### Comparing `earthaccess-0.5.1/earthaccess/__init__.py` & `earthaccess-0.5.2/earthaccess/__init__.py`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.1/earthaccess/api.py` & `earthaccess-0.5.2/earthaccess/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,18 @@
 
     Parameters:
         daac: a DAAC short_name like NSIDC or PODAAC etc
         provider: if we know the provider for the DAAC e.g. POCLOUD, LPCLOUD etc.
     Returns:
         a dictionary with S3 credentials for the DAAC or provider
     """
+    if daac is not None:
+        daac = daac.upper()
+    if provider is not None:
+        provider = provider.upper()
     return earthaccess.__auth__.get_s3_credentials(daac=daac, provider=provider)
 
 
 def collection_query() -> Type[CollectionQuery]:
     """Returns a query builder instance for NASA collections (datasets)
 
     Parameters:
```

### Comparing `earthaccess-0.5.1/earthaccess/auth.py` & `earthaccess-0.5.2/earthaccess/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,16 @@
                     return False
 
         return False
 
     def get_s3_credentials(
         self, daac: Optional[str] = "", provider: Optional[str] = ""
     ) -> Dict[str, str]:
-        """Gets AWS S3 credentials for a given NASA cloud provider
+        """Gets AWS S3 credentials for a given NASA cloud provider, the
+        easier way is to use the DAAC short name. provider is optional if we know it.
 
         Parameters:
             provider: A valid cloud provider, each DAAC has a provider code for their cloud distributions
             daac: the name of a NASA DAAC, i.e. NSIDC or PODAAC
 
         Rreturns:
             A Python dictionary with the temporary AWS S3 credentials
@@ -155,23 +156,34 @@
             auth_url = self._get_cloud_auth_url(daac_shortname=daac, provider=provider)
             if auth_url.startswith("https://"):
                 cumulus_resp = session.get(auth_url, timeout=15, allow_redirects=True)
                 auth_resp = session.get(
                     cumulus_resp.url, allow_redirects=True, timeout=15
                 )
                 if not (auth_resp.ok):  # type: ignore
-                    print(
-                        f"Authentication with Earthdata Login failed with:\n{auth_resp.text[0:1000]}"
+                    # Let's try to authenticate with Bearer tokens
+                    _session = self.get_session()
+                    cumulus_resp = _session.get(
+                        auth_url, timeout=15, allow_redirects=True
                     )
-                    eula_url = "https://urs.earthdata.nasa.gov/users/earthaccess/unaccepted_eulas"
-                    apps_url = "https://urs.earthdata.nasa.gov/application_search"
-                    print(
-                        f"Consider accepting the EULAs available at {eula_url} and applications at {apps_url}"
+                    auth_resp = _session.get(
+                        cumulus_resp.url, allow_redirects=True, timeout=15
                     )
-                    return {}
+                    if not (auth_resp.ok):
+                        print(
+                            f"Authentication with Earthdata Login failed with:\n{auth_resp.text[0:1000]}"
+                        )
+                        eula_url = "https://urs.earthdata.nasa.gov/users/earthaccess/unaccepted_eulas"
+                        apps_url = "https://urs.earthdata.nasa.gov/application_search"
+                        print(
+                            f"Consider accepting the EULAs available at {eula_url} and applications at {apps_url}"
+                        )
+                        return {}
+
+                    return auth_resp.json()
                 return auth_resp.json()
             else:
                 # This happens if the cloud provider doesn't list the S3 credentials or the DAAC
                 # does not have cloud collections yet
                 print(f"Credentials for the cloud provider {daac} are not available")
                 return {}
         else:
```

### Comparing `earthaccess-0.5.1/earthaccess/css/iso_bootstrap4.0.0min.css` & `earthaccess-0.5.2/earthaccess/css/iso_bootstrap4.0.0min.css`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.1/earthaccess/daac.py` & `earthaccess-0.5.2/earthaccess/daac.py`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.1/earthaccess/formatters.py` & `earthaccess-0.5.2/earthaccess/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     {css_inline}
     <div class="bootstrap">
       <div class="container-fluid border">
         <div class="row border">
           <div class="col-6">
             <p><b>Data</b>: {data_links}<p/>
             <p><b>Size</b>: {granule_size} MB</p>
-            <p><b>Spatial</b>: <span>{granule["umm.SpatialExtent"]}</span></p>
+            <p><b>Spatial</b>: <span>{granule["umm"]["SpatialExtent"]}</span></p>
           </div>
           <div class="col-2 offset-sm-3 pull-right">
             {dataviz_img}
           </div>
         </div>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -10,10 +10,10 @@
 """ style = "max-height: 140px;" dataviz_img = "".join( [ f'[Data_Preview]' for
 link in granule.dataviz_links()[0:2] if link.startswith("http") ] ) data_links
 = "".join( [ f'{link.split("/")[-1]}' for link in granule.data_links() ] )
 granule_size = round(granule.size(), 2) # TODO: probably this needs to be
 integrated on a list data structure granule_str = f""" {css_inline}
 Data: {data_links}
 Size: {granule_size} MB
-Spatial: {granule["umm.SpatialExtent"]}
+Spatial: {granule["umm"]["SpatialExtent"]}
 {dataviz_img}
 """ return granule_str
```

### Comparing `earthaccess-0.5.1/earthaccess/results.py` & `earthaccess-0.5.2/earthaccess/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import json
 import uuid
 from typing import Any, Dict, List, Optional, Union
 
-from benedict import benedict
-
 from .formatters import _repr_granule_html
 
 
-class CustomDict(benedict):
+class CustomDict(dict):
     _basic_umm_fields_: List = []
     _basic_meta_fields_: List = []
 
     def __init__(
         self,
         collection: Dict[str, Any],
         fields: Optional[List[str]] = None,
@@ -245,31 +243,30 @@
 
     def size(self) -> float:
         """
         Returns:
             Returns the total size for the granule in MB
         """
         try:
+            data_granule = self["mmm"]["DataGranule"]
             total_size = sum(
                 [
                     float(s["Size"])
-                    for s in self["umm.DataGranule.ArchiveAndDistributionInformation"]
-                    if "ArchiveAndDistributionInformation" in self["umm"]["DataGranule"]
+                    for s in data_granule["ArchiveAndDistributionInformation"]
+                    if "ArchiveAndDistributionInformation" in data_granule
                 ]
             )
         except Exception:
             try:
+                data_granule = self["mmm"]["DataGranule"]
                 total_size = sum(
                     [
                         float(s["SizeInBytes"])
-                        for s in self[
-                            "umm.DataGranule.ArchiveAndDistributionInformation"
-                        ]
-                        if "ArchiveAndDistributionInformation"
-                        in self["umm"]["DataGranule"]
+                        for s in data_granule["ArchiveAndDistributionInformation"]
+                        if "ArchiveAndDistributionInformation" in data_granule
                     ]
                 ) / (1024 * 1024)
             except Exception:
                 total_size = 0
         return total_size
 
     def _derive_s3_link(self, links: List[str]) -> List[str]:
```

### Comparing `earthaccess-0.5.1/earthaccess/search.py` & `earthaccess-0.5.2/earthaccess/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 
 class DataCollections(CollectionQuery):
     """
     ???+ Info
         The DataCollection class queries against https://cmr.earthdata.nasa.gov/search/collections.umm_json,
         the response has to be in umm_json in order to use the result classes.
-        Results will be wraped inside a `Benedict` class, an enhanced Python dictionary.
     """
 
     _fields = None
     _format = "umm_json"
     _valid_formats_regex = [
         "json",
         "xml",
```

### Comparing `earthaccess-0.5.1/earthaccess/store.py` & `earthaccess-0.5.2/earthaccess/store.py`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.1/pyproject.toml` & `earthaccess-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "earthaccess"
-version = "0.5.1"
+version = "0.5.2"
 homepage = "https://github.com/nsidc/earthaccess"
 description = "Client library for NASA Earthdata APIs"
 authors = ["earthaccess contributors"]
 maintainers = [
     "Luis Lopez <betolin@gmail.com>"
 ]
 license = "MIT"
@@ -25,15 +25,14 @@
     "Topic :: Software Development",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 python-cmr = ">=0.7"
-python-benedict = ">=0.25, <0.28.3"
 pqdm = ">=0.1"
 requests = ">=2.26,<3.0.0"
 s3fs = ">=2021.11, <2024"
 fsspec = ">=2022.1"
 tinynetrc = "^1.3.1"
 multimethod = ">=1.8"
```

### Comparing `earthaccess-0.5.1/PKG-INFO` & `earthaccess-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthaccess
-Version: 0.5.1
+Version: 0.5.2
 Summary: Client library for NASA Earthdata APIs
 Home-page: https://github.com/nsidc/earthaccess
 License: MIT
 Author: earthaccess contributors
 Maintainer: Luis Lopez
 Maintainer-email: betolin@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -26,15 +26,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: fsspec (>=2022.1)
 Requires-Dist: multimethod (>=1.8)
 Requires-Dist: pqdm (>=0.1)
-Requires-Dist: python-benedict (>=0.25,<0.28.3)
 Requires-Dist: python-cmr (>=0.7)
 Requires-Dist: requests (>=2.26,<3.0.0)
 Requires-Dist: s3fs (>=2021.11,<2024)
 Requires-Dist: tinynetrc (>=1.3.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
@@ -51,16 +50,16 @@
     <img src="https://img.shields.io/pypi/v/earthaccess?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/earthdata/" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/earthaccess.svg" alt="Python Versions">
 </a>
 
-<a href="https://nsidc.github.io/earthdata/" target="_blank">
-    <img src="https://readthedocs.org/projects/earthaccess/badge/?version=latest&style=plastic" alt="Documentation link">
+<a href='https://earthdata.readthedocs.io/en/latest/?badge=latest'>
+    <img src='https://readthedocs.org/projects/earthdata/badge/?version=latest' alt='Documentation Status' />
 </a>
 
 </p>
 
 ## **Overview**
 
 *earthaccess* is a **python library to search, download or stream NASA Earth science data** with just a few lines of code.
@@ -82,15 +81,15 @@
 
 Using Pip
 
 ```bash
 pip install earthaccess
 ```
 
-Try it in your browser without installing anything! [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nsidc/earthdata/main)
+Try it in your browser without installing anything! [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nsidc/earthaccess/main)
 
 
 ## **Usage**
 
 
 With *earthaccess* we can login, search and download data with a few lines of code and even more relevant, our code will work the same way if we are running it in the cloud or from our laptop. ***earthaccess*** handles authentication with [NASA's Earthdata Login (EDL)](https://urs.earthdata.nasa.gov), search using NASA's [CMR](https://cmr.earthdata.nasa.gov/search/site/docs/search/api.html) and access through [`fsspec`](https://github.com/fsspec/filesystem_spec).
 
@@ -109,17 +108,16 @@
     * if available you can use environment variables **EARTHDATA_USERNAME** and **EARTHDATA_PASSWORD**
 3. Interactively entering your EDL credentials
     * You can be prompted for these credentials and save them to a `.netrc` file
 
 ```python
 import earthaccess
 
-auth = earthaccess.login(strategy="netrc")
-if not auth:
-    auth = earthaccess.login(strategy="interactive", persist=True)
+auth = earthaccess.login()
+
 ```
 
 Once you are authenticated with NASA EDL you can:
 
 * Get a file from a DAAC using a `fsspec` session.
 * Request temporary S3 credentials from a particular DAAC (needed to download or stream data from an S3 bucket in the cloud).
 * Use the library to download or stream data directly from S3.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthaccess Version: 0.5.1 Summary: Client library
+Metadata-Version: 2.1 Name: earthaccess Version: 0.5.2 Summary: Client library
 for NASA Earthdata APIs Home-page: https://github.com/nsidc/earthaccess
 License: MIT Author: earthaccess contributors Maintainer: Luis Lopez
 Maintainer-email: betolin@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Framework :: IPython Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
@@ -11,21 +11,21 @@
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Software Development Classifier:
 Topic :: Software Development :: Libraries Requires-Dist: fsspec (>=2022.1)
 Requires-Dist: multimethod (>=1.8) Requires-Dist: pqdm (>=0.1) Requires-Dist:
-python-benedict (>=0.25,<0.28.3) Requires-Dist: python-cmr (>=0.7) Requires-
-Dist: requests (>=2.26,<3.0.0) Requires-Dist: s3fs (>=2021.11,<2024) Requires-
-Dist: tinynetrc (>=1.3.1,<2.0.0) Description-Content-Type: text/markdown
+python-cmr (>=0.7) Requires-Dist: requests (>=2.26,<3.0.0) Requires-Dist: s3fs
+(>=2021.11,<2024) Requires-Dist: tinynetrc (>=1.3.1,<2.0.0) Description-
+Content-Type: text/markdown
 [earthaccess, a python library to search, download or stream NASA Earth science
                       data with just a few lines of code]
       [Art_Designer:_Allison_Horst] [Package_version] [Python_Versions]
-                             [Documentation_link]
+                            [Documentation_Status]
 ## **Overview** *earthaccess* is a **python library to search, download or
 stream NASA Earth science data** with just a few lines of code. In the age of
 cloud computing, the power of open science only reaches its full potential if
 we have easy-to-use workflows that facilitate research in an inclusive,
 efficient and reproducible way. Unfortunately âas it stands todayâ
 scientists and students alike face a steep learning curve adapting to systems
 that have grown too complex and end up spending more time on the technicalities
@@ -38,75 +38,74 @@
 systems. Therefore, providing easy access to NASA Earthdata regardless of the
 data storage location (hosted within or outside of the cloud) is the main
 motivation behind this Python library. ## **Installing earthaccess** You will
 need Python 3.8 or higher installed. Install the latest release using conda
 ```bash conda install -c conda-forge earthaccess ``` Using Pip ```bash pip
 install earthaccess ``` Try it in your browser without installing anything! [!
 [Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
-nsidc/earthdata/main) ## **Usage** With *earthaccess* we can login, search and
-download data with a few lines of code and even more relevant, our code will
-work the same way if we are running it in the cloud or from our laptop.
+nsidc/earthaccess/main) ## **Usage** With *earthaccess* we can login, search
+and download data with a few lines of code and even more relevant, our code
+will work the same way if we are running it in the cloud or from our laptop.
 ***earthaccess*** handles authentication with [NASA's Earthdata Login (EDL)]
 (https://urs.earthdata.nasa.gov), search using NASA's [CMR](https://
 cmr.earthdata.nasa.gov/search/site/docs/search/api.html) and access through
 [`fsspec`](https://github.com/fsspec/filesystem_spec). The only requirement to
 use this library is to open a free account with NASA [EDL](https://
 urs.earthdata.nasa.gov). [https://auth.ops.maap-project.org/cas/images/urs-
 logo.png] ### **Authentication** Once you have an EDL account, you can
 authenticate using one of the following three methods: 1. Using a `.netrc` file
 * Can use *earthaccess* to read your EDL credentials (username and password)
 from a `.netrc` file 2. Reading your EDL credentials from environment variables
 * if available you can use environment variables **EARTHDATA_USERNAME** and
 **EARTHDATA_PASSWORD** 3. Interactively entering your EDL credentials * You can
 be prompted for these credentials and save them to a `.netrc` file ```python
-import earthaccess auth = earthaccess.login(strategy="netrc") if not auth: auth
-= earthaccess.login(strategy="interactive", persist=True) ``` Once you are
-authenticated with NASA EDL you can: * Get a file from a DAAC using a `fsspec`
-session. * Request temporary S3 credentials from a particular DAAC (needed to
-download or stream data from an S3 bucket in the cloud). * Use the library to
-download or stream data directly from S3. * Regenerate CMR tokens (used for
-restricted datasets) ### **Searching for data** Once we have selected our
-dataset we can search for the data granules using *doi*, *short_name* or
-*concept_id*. If we are not sure or we don't know how to search for a
-particular dataset, we can start with the ["Introducing NASA earthaccess"]
-(https://nsidc.github.io/earthaccess/tutorials/demo/#querying-for-datasets)
-tutorial or through the [NASA Earthdata Search portal](https://
-search.earthdata.nasa.gov/). For a complete list of search parameters we can
-use visit the extended [API documentation](https://nsidc.github.io/earthaccess/
-user-reference/api/api/). ```python results = earthaccess.search_data
-( short_name='ATL06', version="005", cloud_hosted=True, bounding_box=(-10, 20,
-10, 50), temporal=("2020-02", "2020-03"), count=100 ) ``` Now that we have our
-results we can do multiple things: We can iterate over them to get HTTP (or S3)
-links, we can download the files to a local folder, or we can open these files
-and stream their content directly to other libraries e.g. xarray. ###
-**Accessing the data** **Option 1: Using the data links** If we already have a
-workflow in place for downloading our data, we can use *earthaccess* as a
-search-only library and get HTTP links from our query results. This could be
-the case if our current workflow uses a different language and we only need the
-links as input. ```python # if the data set is cloud hosted there will be S3
-links available. The access parameter accepts "direct" or "external", direct
-access is only possible if you are in the us-west-2 region in the cloud.
-data_links = [granule.data_links(access="direct") for granule in results] # or
-if the data is an on-prem dataset data_links = [granule.data_links
-(access="external") for granule in results] ``` > Note: *earthaccess* can get
-S3 credentials for us, or auhenticated HTTP sessions in case we want to use
-them with a different library. **Option 2: Download data to a local folder**
-This option is practical if you have the necessary space available on disk. The
-*earthaccess* library will print out the approximate size of the download and
-its progress. ```python files = earthaccess.download(results, "./local_folder")
-``` **Option 3: Direct S3 Access - Stream data directly to xarray** This method
-works best if you are in the same Amazon Web Services (AWS) region as the data
-(us-west-2) and you are working with gridded datasets (processing level 3 and
-above). ```python import xarray as xr ds = xr.open_mfdataset(earthaccess.open
-(results)) ``` And that's it! Just one line of code, and this same piece of
-code will also work for data that are not hosted in the cloud, i.e. located at
-NASA storage centers. > More examples coming soon! ### Compatibility Only
-**Python 3.8+** is supported. ## Contributors [![Contributors](https://
-contrib.rocks/image?repo=nsidc/earthaccess)](https://github.com/nsidc/
-earthaccess/graphs/contributors) ## Contributing Guide Welcome! ðð >
-Please see the [Contributing Guide](CONTRIBUTING.md). ### [Project Board]
-(https://github.com/nsidc/earthdata/discussions). ### Glossary NASA_Earth
-Science_Glossary ## License earthaccess is licensed under the MIT license. See
-[LICENSE](LICENSE.txt). ## Level of Support
+import earthaccess auth = earthaccess.login() ``` Once you are authenticated
+with NASA EDL you can: * Get a file from a DAAC using a `fsspec` session. *
+Request temporary S3 credentials from a particular DAAC (needed to download or
+stream data from an S3 bucket in the cloud). * Use the library to download or
+stream data directly from S3. * Regenerate CMR tokens (used for restricted
+datasets) ### **Searching for data** Once we have selected our dataset we can
+search for the data granules using *doi*, *short_name* or *concept_id*. If we
+are not sure or we don't know how to search for a particular dataset, we can
+start with the ["Introducing NASA earthaccess"](https://nsidc.github.io/
+earthaccess/tutorials/demo/#querying-for-datasets) tutorial or through the
+[NASA Earthdata Search portal](https://search.earthdata.nasa.gov/). For a
+complete list of search parameters we can use visit the extended [API
+documentation](https://nsidc.github.io/earthaccess/user-reference/api/api/).
+```python results = earthaccess.search_data( short_name='ATL06', version="005",
+cloud_hosted=True, bounding_box=(-10, 20, 10, 50), temporal=("2020-02", "2020-
+03"), count=100 ) ``` Now that we have our results we can do multiple things:
+We can iterate over them to get HTTP (or S3) links, we can download the files
+to a local folder, or we can open these files and stream their content directly
+to other libraries e.g. xarray. ### **Accessing the data** **Option 1: Using
+the data links** If we already have a workflow in place for downloading our
+data, we can use *earthaccess* as a search-only library and get HTTP links from
+our query results. This could be the case if our current workflow uses a
+different language and we only need the links as input. ```python # if the data
+set is cloud hosted there will be S3 links available. The access parameter
+accepts "direct" or "external", direct access is only possible if you are in
+the us-west-2 region in the cloud. data_links = [granule.data_links
+(access="direct") for granule in results] # or if the data is an on-prem
+dataset data_links = [granule.data_links(access="external") for granule in
+results] ``` > Note: *earthaccess* can get S3 credentials for us, or
+auhenticated HTTP sessions in case we want to use them with a different
+library. **Option 2: Download data to a local folder** This option is practical
+if you have the necessary space available on disk. The *earthaccess* library
+will print out the approximate size of the download and its progress. ```python
+files = earthaccess.download(results, "./local_folder") ``` **Option 3: Direct
+S3 Access - Stream data directly to xarray** This method works best if you are
+in the same Amazon Web Services (AWS) region as the data (us-west-2) and you
+are working with gridded datasets (processing level 3 and above). ```python
+import xarray as xr ds = xr.open_mfdataset(earthaccess.open(results)) ``` And
+that's it! Just one line of code, and this same piece of code will also work
+for data that are not hosted in the cloud, i.e. located at NASA storage
+centers. > More examples coming soon! ### Compatibility Only **Python 3.8+** is
+supported. ## Contributors [![Contributors](https://contrib.rocks/
+image?repo=nsidc/earthaccess)](https://github.com/nsidc/earthaccess/graphs/
+contributors) ## Contributing Guide Welcome! ðð > Please see the
+[Contributing Guide](CONTRIBUTING.md). ### [Project Board](https://github.com/
+nsidc/earthdata/discussions). ### Glossary NASA_Earth_Science_Glossary ##
+License earthaccess is licensed under the MIT license. See [LICENSE]
+(LICENSE.txt). ## Level of Support
 [https://raw.githubusercontent.com/nsidc/earthdata/main/docs/nsidc-logo.png]
 This repository is not actively supported by NSIDC but we welcome issue
 submissions and pull requests in order to foster community contribution.
```

