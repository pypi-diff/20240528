# Comparing `tmp/iso3166_updates-1.7.0.tar.gz` & `tmp/iso3166_updates-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166_updates-1.7.0.tar", max compression
+gzip compressed data, was "iso3166_updates-1.7.1.tar", max compression
```

## Comparing `iso3166_updates-1.7.0.tar` & `iso3166_updates-1.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1059 2024-04-18 21:29:13.496417 iso3166_updates-1.7.0/LICENSE
--rw-r--r--   0        0        0    26210 2024-04-18 21:29:13.496417 iso3166_updates-1.7.0/README.md
--rw-r--r--   0        0        0     2794 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/iso3166_updates/README.md
--rw-r--r--   0        0        0      803 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/iso3166_updates/__init__.py
--rw-r--r--   0        0        0   369134 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/iso3166_updates/iso3166-updates.json
--rw-r--r--   0        0        0    25216 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/iso3166_updates/iso3166_updates.py
--rw-r--r--   0        0        0     1873 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    27994 1970-01-01 00:00:00.000000 iso3166_updates-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-28 19:57:56.624184 iso3166_updates-1.7.1/LICENSE
+-rw-r--r--   0        0        0    27570 2024-05-28 19:57:56.624184 iso3166_updates-1.7.1/README.md
+-rw-r--r--   0        0        0     2806 2024-05-28 19:57:56.628185 iso3166_updates-1.7.1/iso3166_updates/README.md
+-rw-r--r--   0        0        0      803 2024-05-28 19:57:56.628185 iso3166_updates-1.7.1/iso3166_updates/__init__.py
+-rw-r--r--   0        0        0   369135 2024-05-28 19:57:56.632185 iso3166_updates-1.7.1/iso3166_updates/iso3166-updates.json
+-rw-r--r--   0        0        0    25216 2024-05-28 19:57:56.632185 iso3166_updates-1.7.1/iso3166_updates/iso3166_updates.py
+-rw-r--r--   0        0        0     1906 2024-05-28 19:57:56.632185 iso3166_updates-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    29408 1970-01-01 00:00:00.000000 iso3166_updates-1.7.1/PKG-INFO
```

### Comparing `iso3166_updates-1.7.0/LICENSE` & `iso3166_updates-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166_updates-1.7.0/README.md` & `iso3166_updates-1.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 <!-- [![codecov](https://codecov.io/gh/amckenna41/iso3166-updates/graph/badge.svg?token=XOBSBVH8XA)](https://codecov.io/gh/amckenna41/iso3166-updates) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
   <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
 </div>
 
-> Software and API that checks for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package as well as an API. 
+> Software and accompanying API that checks for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package as well as an API. 
 
 * A <b>demo</b> of the software and API is available [here][demo_iso3166_updates].
 * A <b>demo</b> of the script used to pull and export all the latest updates is available [here][demo_get_all_iso3166_updates].
 * A <b>Medium</b> article that dives deeper into `iso3166-updates` is available [here][medium].
 * The front-end <b>API</b> is available [here][api].
 * The **documentation** for the software is available [here](https://iso3166-updates.readthedocs.io/en/latest/).
 
@@ -40,19 +40,19 @@
 - [Contact](#contact)
 - [References](#references)
 
 Introduction
 ------------
 `iso3166-updates` is a software and accompanying API that consists of a series of scripts that check for any updates/changes to the ISO 3166 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui).
 
-The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations 🇺🇳 [[1]](#references). The ISO 3166-2 was first published in 1998 and as of November 2023 there are 5,039 codes defined in it [[2]](#references).
+The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions etc), which comprise the ISO 3166-2 standard [[2]](#references). The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations 🇺🇳 [[1]](#references). The ISO 3166-2 was first published in 1998 and as of November 2023 there are **5,039** codes defined in it [[2]](#references).
 
 ### Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with and track these changes. These changes can occur for a variety of geopolitical and administrative reasons. Previously these changes were communicated via newsletters; but as of July 2013 these changes are now communicated via their online catalogue/Online Browsing Platform (OBP), or via a database, which usually costs money to subscribe to (up to $300) [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change, update and or remove entries within its library of standards, including the ISO 3166. Additions, changes and or deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with and track these changes. These changes can occur for a variety of geopolitical and administrative reasons. Previously these changes were communicated via newsletters; but as of July 2013 these changes are now communicated via their online catalogue/Online Browsing Platform (OBP), or via a database, which usually costs money to subscribe to (**up to $300**) [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API make it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free; with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
 ### Intended Audience:
 
 This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
@@ -73,60 +73,62 @@
 * https://iso3166-updates.com/api/alpha/<input_alpha>
 * https://iso3166-updates.com/api/name/<input_name>
 * https://iso3166-updates.com/api/year/<input_year>
 * https://iso3166-updates.com/api/alpha/<input_alpha>/year/<input_year>
 * https://iso3166-updates.com/api/name/<input_name>/year/<input_year>
 * https://iso3166-updates.com/api/months/<input_month>
 * https://iso3166-updates.com/api/months/<input_month>/alpha/<input_alpha>
+* https://iso3166-updates.com/api/months/<input_month>/name/<input_name>
 
-The paths/endpoints available in the API are - `/api/all`, `/api/alpha`, `/api/name`, `/api/year` and `/api/months`. 
+The main paths/endpoints available in the API are - `/api/all`, `/api/alpha`, `/api/name`, `/api/year` and `/api/months`. 
 
 * `/api/all`: get all of the ISO 3166 updates/changes data for all countries.
 
 * `/api/alpha`: get all the ISO 3166 updates/changes data for one or more countries according to their ISO 3166-1 alpha-2, alpha-3 or numeric country codes. A single alpha code or a list of them can be passed to the API e.g. `/api/alpha/AL`, `/api/alpha/BW`, `/api/alpha/FR,DE,HUN,IDN,504`. If an invalid alpha code is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **month** endpoints to get the country updates for a specific country and year, and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/alpha/<input_alpha>/year/<input_year>` and `/api/alpha/<input_alpha>/months/<input_month>`, respectively.
 
-* `/api/name`: get all the ISO 3166 updates/changes data for one or more countries according to their country name, as listed in the ISO 3166-1. A single country name or list of them can be passed into the API e.g. `/api/name/Brazil`, `/api/name/Colombia`, `/api/name/Benin,France,Moldova`. A closeness function is used to get the most approximate available country from the one input, e.g. Sweden will be used if the input is `/api/name/Swede`. If no matching country is found from the closeness function or an invalid name is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **months** endpoint to get the country updates for a specific country name and year and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/name/<input_name>/year/<input_year>` and `/api/name/<input_name>/months/<input_month>`, respectively. 
+* `/api/name`: get all the ISO 3166 updates/changes data for one or more countries according to their country name, as listed in the ISO 3166-1. A single country name or list of them can be passed to the API e.g. `/api/name/Brazil`, `/api/name/Colombia`, `/api/name/Benin,France,Moldova`. A closeness function is used to get the most approximate available country from the one input, e.g. Sweden will be used if the input is `/api/name/Swede`. If no matching country is found from the closeness function or an invalid name is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **months** endpoint to get the country updates for a specific country name and year and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/name/<input_name>/year/<input_year>` and `/api/name/<input_name>/months/<input_month>`, respectively. 
 
 * `/api/year`: get all the ISO 3166 updates/changes data for one or more countries according to a specific year, year range, or a cut-off year to get updates less than/more than a year, e.g. `/api/year/2017`, `/api/year/2010-2015`, `/api/year/<2009`, `/api/year/>2002`. If an invalid year is input then an error will be returned. This endpoint can be used in conjunction with the **alpha** and **name** endpoints to get the country updates for a specific country and year. This will be in in the format `/api/alpha/<input_alpha>/year/<input_year>` and `/api/name/<input_name>/year/<input_year>`, respectively. 
 
 * `/api/months`: get all the ISO 3166 updates/changes data for one or more countries from an input number of months from the present day, e.g. `/api/months/12`, `/api/months/24`, `/api/months/50`. A month range can also be input to get the updates published within a specified range of months, with the start and end month separated by a '-' e.g. `/api/months/12-24`, `/api/months/36-50`. If an invalid month value is input then an error will be returned. This endpoint can be used in conjunction with the **alpha** and **name** endpoints to get the country updates for a specific country over the past number of months using their ISO 3166-1 alpha code or country name, respectively. This will be in the format: `/api/months/<input_month>/alpha/<input_alpha>` and `/api/months/<input_month>/name/<input_name>`, respectively.
 
 * `/api`: main homepage and API documentation.
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
+The API was originally hosted and built using GCP, with a Cloud Function being used in the backend, fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
 
 The full list of attributes available for each country are:
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
-* Date Issued: date that the change was communicated.
 * Code/Subdivision change: overall summary of change/update made.
 * Description of change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Date Issued: date that the change was communicated.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
 
 Documentation
 -------------
 Documentation for the software and accompanying API is available on the software's [readthedocs](https://iso3166-updates.readthedocs.io/en/latest/) page. Additionally the API's documentation is available on the API [homepage](https://iso3166-updates.com/api). A demo of both is also available [here][demo_iso3166_updates].
 
 <!-- <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_architecture.png?raw=true" alt="gcp_arch" height="500" width="750"/>
 </p> -->
 
 Staying up to date
 ------------------
 The list of ISO 3166 updates was last updated on <strong>March 2024</strong>.
 
-The object storing all updates - iso3166-updates.json - for the software package is consistently checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes from the various data sources, to check for the latest updates within a certain period e.g. the past 6-12 months (this month range is used as the ISO usually publishes their updates at the end of the year with occasional mid-year updates). The app compares the generated output with that of the updates JSON currently in the software package and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to call the application on the aforementioned schedule. 
+The object storing all updates - iso3166-updates.json - for the software package is consistently checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes from the various data sources, to check for the latest updates within a certain period e.g. the past 6-12 months (this month range is used as the ISO usually publishes their updates at the end of the year with occasional mid-year updates). The app compares the generated output with that of the updates JSON currently in the software package and will replace this json to integrate the latest updates found, such that the API will have the most **up-to-date** and **accurate** data. A Cloud Scheduler is used to call the application on the aforementioned schedule. 
 
 Additionally, a GitHub Issue in the custom-built [`iso3166-updates`](https://github.com/amckenna41/iso3166-updates), [`iso3166-2`](https://github.com/amckenna41/iso3166-2) and [`iso3166-flag-icons`](https://github.com/amckenna41/iso3166-flag-icons) repositories will be automatically created that formats and tabulates all updates/changes that need to be implemented into the JSONs on the aforementioned repos.
 
-Ultimately, this Cloud Run microservice ensures that the software and associated APIs are up-to-date with the most latest, accurate and reliable ISO 3166-2 information for all countries/territories/subdivisions etc.
+Ultimately, this Cloud Run microservice ensures that the software and associated APIs are up-to-date with the **most latest, accurate** and **reliable** ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
 * [python][python] >= 3.8
 * [iso3166][iso3166] >= 2.1.1 
+* [python-dateutil][python-dateutil] >= 2.9.0
 
 Installation
 ------------
 Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-updates --upgrade
@@ -157,25 +159,25 @@
 ```
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY:**
 ```python
 iso["BA","DE","FRA","HUN","600"]
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2003 and 2004:**
+**Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2005 and 2009:**
 ```python
-iso.year("2002, 2003, 2004")
+iso.year("2002, 2005, 2009")
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016:**
+**Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016, inclusive:**
 ```python
 iso.year("2013-2016")
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for all years after 2017 inclusive:**
+**Get all listed ISO 3166 changes/updates for all countries, for all years after 2017, inclusive:**
 ```python
 iso.year(">2017")
 ```
 
 **Get any listed ISO 3166 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
 iso.year("2012-2021").IE
@@ -243,23 +245,23 @@
   # -verbose VERBOSE, --verbose VERBOSE
   #                       Set to 1 to print out progress of updates function, 0 will not print progress (default=True).
   # -use_selenium USE_SELENIUM, --use_selenium USE_SELENIUM
   #                       Gather all data for each country from its official page on the ISO website which 
   #                       requires Python Selenium and Chromedriver. If False then just use country data
   #                       from its wiki page (default=True).
 ```
-**Get all the latest updates for all ISO 3166 countries**
+<!-- **Get all the latest updates for all ISO 3166 countries:**
 ```bash
 ./get_all_updates.sh 
 
 '''
---export_filename     Filename for exported JSON/CSV files containing updates data (default="iso3166-updates.json").
+--export_filename     Filename for exported JSON/CSV files containing updates data (default="iso3166-updates").
 --export_folder       Folder name to store exported JSON/CSV files containing updates data (default="test-iso3166-updates).
 '''
-```
+``` -->
 
 <!-- **Import module:**
 ```python
 import get_all_iso3166_updates as iso3166_updates
 ```
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
@@ -289,74 +291,84 @@
 **Get any listed ISO 3166 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ``` -->
 
 The output files from the <i>get_all_iso3166_updates.py</i> script for the updates/changes to an ISO 3166-2 country returns 4 columns: 
-<b>Edition/Newsletter, Date Issued, Code/Subdivision Change</b> and <b>Description of Change.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+<b>Code/Subdivision Change, Description of Change, Date Issued</b> and <b>Edition/Newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
-* Date Issued: date that the change was communicated.
 * Code/Subdivision Change: overall summary of change/update made.
 * Description of Change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Date Issued: date that the change was communicated.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
 
 E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
-| Edition/Newsletter | Date Issued | Code/Subdivision Change | Description of Change |   
+| Code/Subdivision Change | Description of Change | Date Issued | Edition/Newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
-| Newsletter I-8.    | 2007-04-17  | Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements.                 | 
-| Online Browsing Platform (OBP). | 2014-11-03 | | Update List Source |
-| Online Browsing Platform (OBP). | 2015-11-27 | | Update List Source | 
+| Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements. | 2007-04-17 | Newsletter I-8. | 
+| Update List Source. |  | 2014-11-03 | Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AD) | 
+| Update List Source. |  | 2015-11-27 | Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AD) | 
 
 E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   "AD": [
       {
-          "Date Issued": "2015-11-27",
-          "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD).",
           "Code/Subdivision Change": "Update List Source.",
-          "Description of Change": ""
+          "Description of Change": "",
+          "Date Issued": "2015-11-27",
+          "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)."
       },
       {
-          "Date Issued": "2014-11-03",
-          "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD).",
           "Code/Subdivision Change": "Update List Source.",
-          "Description of Change": ""
+          "Description of Change": "",
+          "Date Issued": "2014-11-03",
+          "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)."
       },
       {
-          "Date Issued": "2007-04-17",
-          "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf).",
           "Code/Subdivision Change": "Subdivisions added: 7 parishes.",
-          "Description of Change": "Addition of the administrative subdivisions and of their code elements."
+          "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
+          "Date Issued": "2007-04-17",
+          "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
+
       }
   ]
 }
 ```
 
 Directories 
 -----------
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Run microservice for the check-for-updates function which is a periodically called Cloud Run app that uses the Python software to check for the latest updates for all ISO 3166 countries, ensuring the API and jsons are reliable, accurate and up-to-date.
 * `/docs` - documentation for `iso3166-updates`, available on [readthedocs](https://iso3166-updates.readthedocs.io/en/latest/).
 * `/tests` - unit and integration tests for `iso3166-updates` software and API.
 * `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
-* `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium. 
+<!-- * `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium.  -->
 * `UPDATES.md` - log of all the latest updates from 2022 onwards. 
 
 Issues
 ------
 Any issues, errors/bugs or enhancements can be raised via the [Issues][Issues] tab in the repository.
 
 Contact 
 -------
 If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
 <!-- [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/) -->
 
+Other ISO 3166 repositories
+---------------------------
+Below are some of my other custom-built repositories that relate to the ISO 3166 standard.
+
+* [iso3166-updates-api](https://github.com/amckenna41/iso3166-updates-api): frontend API for iso3166-updates.
+* [iso3166-2](https://github.com/amckenna41/iso3166-2): a lightweight custom-built Python package, and accompanying API, that can be used to access all of the world's ISO 3166-2 subdivision data. A plethora of data attributes are available per country and subdivision including: name, local name, code, parent code, type, lat/longitude and flag. Currently, the package and API supports data from 250 countries/territories, according to the ISO 3166-1 standard.
+* [iso3166-2-api](https://github.com/amckenna41/iso3166-2-api): frontend API for iso3166-2.
+* [iso3166-flag-icons](https://github.com/amckenna41/iso3166-flag-icons): a comprehensive library of over 3500 country and regional flags from the ISO 3166-1 and ISO 3166-2 standards.
+
 References
 ----------
 \[1\]: ISO 3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
 \[2\]: ISO 3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
 \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
 \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
 \[5\]: ISO 3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
@@ -370,24 +382,25 @@
 
 [demo_iso3166_updates]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [demo_get_all_iso3166_updates]: https://colab.research.google.com/drive/161aclDjGkWQJhis7KxBO1e6H_ghQOPRG?usp=sharing
 [api]: https://www.iso3166-updates.com/api
 [medium]: https://medium.com/@ajmckenna69/iso3166-updates-d06b817af3a7
 [python]: https://www.python.org/downloads/release/python-360/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
+[python-dateutil]: https://pypi.org/project/python-dateutil/
 [pandas]: https://pandas.pydata.org/
 [tqdm]: https://github.com/tqdm/tqdm
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [google-auth]: https://cloud.google.com/python/docs/reference
 [google-cloud-storage]: https://cloud.google.com/python/docs/reference
 [google-api-python-client]: https://cloud.google.com/python/docs/reference
 [flask]: https://flask.palletsprojects.com/en/2.3.x/
 [emoji-country-flag]: https://pypi.org/project/emoji-country-flag/
 [gunicorn]: https://pypi.org/project/gunicorn/
 [selenium]: https://selenium-python.readthedocs.io/index.html
 [webdriver-manager]: https://pypi.org/project/webdriver-manager/
 [lxml]: https://lxml.de/
-[updates_md]: https://github.com/amckenna41/iso3166-updates/blob/main/UPDATES.md
+[updates_md]: https://github.com/amckenna41/iso3166-updates/blob/main/UPDATES.MD
 [iso3166]: https://github.com/deactivated/python-iso3166
 [PyPi]: https://pypi.org/project/iso3166-updates/
 [Issues]: https://github.com/amckenna41/iso3166-updates/issues
```

### Comparing `iso3166_updates-1.7.0/iso3166_updates/README.md` & `iso3166_updates-1.7.1/iso3166_updates/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,25 +32,25 @@
 ```
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FRA, HUN, PY (600):**
 ```python
 iso["BA","DE","FRA","HUN","600"]
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2003 and 2004:**
+**Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2005 and 2009:**
 ```python
-iso.year("2002, 2003, 2004")
+iso.year("2002, 2005, 2009")
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016:**
+**Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016, inclusive:**
 ```python
 iso.year("2013-2016")
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for all years after 2017 inclusive:**
+**Get all listed ISO 3166 changes/updates for all countries, for all years after 2017, inclusive:**
 ```python
 iso.year(">2017")
 ```
 
 **Get all listed ISO 3166 changes/updates for all countries, for all years before 2010:**
 ```python
 iso.year("<2010")
@@ -64,11 +64,11 @@
 **Get all listed ISO 3166 changes/updates published from the past 36-48 months:**
 ```python
 iso.months("36-48")
 ```
 
 The output to the above functions for the updates/changes to an ISO 3166 country returns 4 attributes: 
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
-* Date Issued: date that the change was communicated.
 * Code/Subdivision change: overall summary of change/update made.
-* Description of Change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Description of Change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Date Issued: date that the change was communicated.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
```

### Comparing `iso3166_updates-1.7.0/iso3166_updates/__init__.py` & `iso3166_updates-1.7.1/iso3166_updates/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .iso3166_updates import *
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 __description__ = "Get the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Production'
```

### Comparing `iso3166_updates-1.7.0/iso3166_updates/iso3166-updates.json` & `iso3166_updates-1.7.1/iso3166_updates/iso3166-updates.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999968624497992%*

 * *Differences: {"'IR'": "{0: {'Code/Subdivision Change': 'Change of short name upper case: replace the "*

 * *         "parentheses with a comma.'}}"}*

```diff
@@ -2677,15 +2677,15 @@
             "Date Issued": "2014-10-30",
             "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IQ)."
         }
     ],
     "IR": [
         {
-            "Code/Subdivision Change": "Change of short name upper case: replace the parentheses with a coma.",
+            "Code/Subdivision Change": "Change of short name upper case: replace the parentheses with a comma.",
             "Date Issued": "2024-02-29",
             "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IR)."
         },
         {
             "Code/Subdivision Change": "Change of subdivision code from IR-01 to IR-03, IR-02 to IR-04, IR-03 to IR-24, IR-04 to IR-10, IR-05 to IR-16, IR-06 to IR-18, IR-07 to IR-23, IR-08 to IR-14, IR-10 to IR-06, IR-11 to IR-19, IR-12 to IR-20, IR-13 to IR-11, IR-14 to IR-07, IR-15 to IR-08, IR-16 to IR-12, IR-17 to IR-05, IR-18 to IR-17, IR-19 to IR-01, IR-20 to IR-15, IR-21 to IR-02, IR-22 to IR-00, IR-23 to IR-22, IR-24 to IR-13, IR-25 to IR-21, IR-26 to IR-25, IR-28 to IR-26, IR-30 to IR-09, IR-31 to IR-28, IR-32 to IR-30; Update Code Source.",
             "Date Issued": "2020-11-24",
```

### Comparing `iso3166_updates-1.7.0/iso3166_updates/iso3166_updates.py` & `iso3166_updates-1.7.1/iso3166_updates/iso3166_updates.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import platform
 
 class ISO3166_Updates():
     """
     This class is used to access all the ISO-3166 updates/changes data from its respective json
     created from the data sources used in the get_all_iso3166_updates.py script. All of the 
     keys and objects in the JSON are accessible via dot notation using the Map class. Each
-    country has the attributes: Date Issued, Edition/Newsletter, Code/Subdivision Change and
-    Description of Change. 
+    country has the attributes: Code/Subdivision Change, Description of Change, Date Issued and 
+    Edition/Newsletter.
     
     "Date Issued" is the date at which the change was published by the ISO, the "Edition/Newsletter"
     column is the name and or edition of newsletter that the ISO 3166 change/update was communicated 
     in, "Code/Subdivision Change" column is the overall summary of change/update made and 
     "Description of Change" is a more in-depth info about the change/update that was made.
 
     Currently there are 249 country's listed in the updates json with updates dating from 2000 up
```

### Comparing `iso3166_updates-1.7.0/pyproject.toml` & `iso3166_updates-1.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "iso3166-updates"
-version = "1.7.0"
+version = "1.7.1"
 description = "Get the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest." 
-authors = ["AJ Mckenna <amckenna41@qub.ac.uk>"]
+authors = ["AJ McKenna <amckenna41@qub.ac.uk>"]
 maintainers = ["AJ McKenna <amckenna41@qub.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
@@ -27,14 +27,15 @@
 ]
 keywords = ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "csv", "iso3166-2", "subdivisions", "iso3166-1", "alpha-2", "alpha-3", "selenium", "chromedriver"]
 packages = [{include = "iso3166_updates"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 iso3166 = "^2.1.1"
+python-dateutil = "^2.9.0.post0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 
 [tool.poetry.urls]
 homepage = "https://iso3166-updates.com/api/"
 repository = "https://github.com/amckenna41/iso3166-updates"
```

### Comparing `iso3166_updates-1.7.0/PKG-INFO` & `iso3166_updates-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.7.0
+Version: 1.7.1
 Summary: Get the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest.
 License: MIT
 Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,subdivisions,iso3166-1,alpha-2,alpha-3,selenium,chromedriver
-Author: AJ Mckenna
+Author: AJ McKenna
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 Maintainer-email: amckenna41@qub.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: iso3166 (>=2.1.1,<3.0.0)
+Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Project-URL: documentation, https://iso3166-updates.readthedocs.io/en/latest/
 Project-URL: homepage, https://iso3166-updates.com/api/
 Project-URL: repository, https://github.com/amckenna41/iso3166-updates
 Description-Content-Type: text/markdown
 
 # iso3166-updates 🌎
 
@@ -49,15 +50,15 @@
 <!-- [![codecov](https://codecov.io/gh/amckenna41/iso3166-updates/graph/badge.svg?token=XOBSBVH8XA)](https://codecov.io/gh/amckenna41/iso3166-updates) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
   <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
 </div>
 
-> Software and API that checks for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package as well as an API. 
+> Software and accompanying API that checks for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package as well as an API. 
 
 * A <b>demo</b> of the software and API is available [here][demo_iso3166_updates].
 * A <b>demo</b> of the script used to pull and export all the latest updates is available [here][demo_get_all_iso3166_updates].
 * A <b>Medium</b> article that dives deeper into `iso3166-updates` is available [here][medium].
 * The front-end <b>API</b> is available [here][api].
 * The **documentation** for the software is available [here](https://iso3166-updates.readthedocs.io/en/latest/).
 
@@ -76,19 +77,19 @@
 - [Contact](#contact)
 - [References](#references)
 
 Introduction
 ------------
 `iso3166-updates` is a software and accompanying API that consists of a series of scripts that check for any updates/changes to the ISO 3166 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui).
 
-The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations 🇺🇳 [[1]](#references). The ISO 3166-2 was first published in 1998 and as of November 2023 there are 5,039 codes defined in it [[2]](#references).
+The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions etc), which comprise the ISO 3166-2 standard [[2]](#references). The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations 🇺🇳 [[1]](#references). The ISO 3166-2 was first published in 1998 and as of November 2023 there are **5,039** codes defined in it [[2]](#references).
 
 ### Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with and track these changes. These changes can occur for a variety of geopolitical and administrative reasons. Previously these changes were communicated via newsletters; but as of July 2013 these changes are now communicated via their online catalogue/Online Browsing Platform (OBP), or via a database, which usually costs money to subscribe to (up to $300) [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change, update and or remove entries within its library of standards, including the ISO 3166. Additions, changes and or deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with and track these changes. These changes can occur for a variety of geopolitical and administrative reasons. Previously these changes were communicated via newsletters; but as of July 2013 these changes are now communicated via their online catalogue/Online Browsing Platform (OBP), or via a database, which usually costs money to subscribe to (**up to $300**) [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API make it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free; with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
 ### Intended Audience:
 
 This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
@@ -109,60 +110,62 @@
 * https://iso3166-updates.com/api/alpha/<input_alpha>
 * https://iso3166-updates.com/api/name/<input_name>
 * https://iso3166-updates.com/api/year/<input_year>
 * https://iso3166-updates.com/api/alpha/<input_alpha>/year/<input_year>
 * https://iso3166-updates.com/api/name/<input_name>/year/<input_year>
 * https://iso3166-updates.com/api/months/<input_month>
 * https://iso3166-updates.com/api/months/<input_month>/alpha/<input_alpha>
+* https://iso3166-updates.com/api/months/<input_month>/name/<input_name>
 
-The paths/endpoints available in the API are - `/api/all`, `/api/alpha`, `/api/name`, `/api/year` and `/api/months`. 
+The main paths/endpoints available in the API are - `/api/all`, `/api/alpha`, `/api/name`, `/api/year` and `/api/months`. 
 
 * `/api/all`: get all of the ISO 3166 updates/changes data for all countries.
 
 * `/api/alpha`: get all the ISO 3166 updates/changes data for one or more countries according to their ISO 3166-1 alpha-2, alpha-3 or numeric country codes. A single alpha code or a list of them can be passed to the API e.g. `/api/alpha/AL`, `/api/alpha/BW`, `/api/alpha/FR,DE,HUN,IDN,504`. If an invalid alpha code is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **month** endpoints to get the country updates for a specific country and year, and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/alpha/<input_alpha>/year/<input_year>` and `/api/alpha/<input_alpha>/months/<input_month>`, respectively.
 
-* `/api/name`: get all the ISO 3166 updates/changes data for one or more countries according to their country name, as listed in the ISO 3166-1. A single country name or list of them can be passed into the API e.g. `/api/name/Brazil`, `/api/name/Colombia`, `/api/name/Benin,France,Moldova`. A closeness function is used to get the most approximate available country from the one input, e.g. Sweden will be used if the input is `/api/name/Swede`. If no matching country is found from the closeness function or an invalid name is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **months** endpoint to get the country updates for a specific country name and year and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/name/<input_name>/year/<input_year>` and `/api/name/<input_name>/months/<input_month>`, respectively. 
+* `/api/name`: get all the ISO 3166 updates/changes data for one or more countries according to their country name, as listed in the ISO 3166-1. A single country name or list of them can be passed to the API e.g. `/api/name/Brazil`, `/api/name/Colombia`, `/api/name/Benin,France,Moldova`. A closeness function is used to get the most approximate available country from the one input, e.g. Sweden will be used if the input is `/api/name/Swede`. If no matching country is found from the closeness function or an invalid name is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **months** endpoint to get the country updates for a specific country name and year and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/name/<input_name>/year/<input_year>` and `/api/name/<input_name>/months/<input_month>`, respectively. 
 
 * `/api/year`: get all the ISO 3166 updates/changes data for one or more countries according to a specific year, year range, or a cut-off year to get updates less than/more than a year, e.g. `/api/year/2017`, `/api/year/2010-2015`, `/api/year/<2009`, `/api/year/>2002`. If an invalid year is input then an error will be returned. This endpoint can be used in conjunction with the **alpha** and **name** endpoints to get the country updates for a specific country and year. This will be in in the format `/api/alpha/<input_alpha>/year/<input_year>` and `/api/name/<input_name>/year/<input_year>`, respectively. 
 
 * `/api/months`: get all the ISO 3166 updates/changes data for one or more countries from an input number of months from the present day, e.g. `/api/months/12`, `/api/months/24`, `/api/months/50`. A month range can also be input to get the updates published within a specified range of months, with the start and end month separated by a '-' e.g. `/api/months/12-24`, `/api/months/36-50`. If an invalid month value is input then an error will be returned. This endpoint can be used in conjunction with the **alpha** and **name** endpoints to get the country updates for a specific country over the past number of months using their ISO 3166-1 alpha code or country name, respectively. This will be in the format: `/api/months/<input_month>/alpha/<input_alpha>` and `/api/months/<input_month>/name/<input_name>`, respectively.
 
 * `/api`: main homepage and API documentation.
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
+The API was originally hosted and built using GCP, with a Cloud Function being used in the backend, fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
 
 The full list of attributes available for each country are:
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
-* Date Issued: date that the change was communicated.
 * Code/Subdivision change: overall summary of change/update made.
 * Description of change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Date Issued: date that the change was communicated.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
 
 Documentation
 -------------
 Documentation for the software and accompanying API is available on the software's [readthedocs](https://iso3166-updates.readthedocs.io/en/latest/) page. Additionally the API's documentation is available on the API [homepage](https://iso3166-updates.com/api). A demo of both is also available [here][demo_iso3166_updates].
 
 <!-- <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_architecture.png?raw=true" alt="gcp_arch" height="500" width="750"/>
 </p> -->
 
 Staying up to date
 ------------------
 The list of ISO 3166 updates was last updated on <strong>March 2024</strong>.
 
-The object storing all updates - iso3166-updates.json - for the software package is consistently checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes from the various data sources, to check for the latest updates within a certain period e.g. the past 6-12 months (this month range is used as the ISO usually publishes their updates at the end of the year with occasional mid-year updates). The app compares the generated output with that of the updates JSON currently in the software package and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to call the application on the aforementioned schedule. 
+The object storing all updates - iso3166-updates.json - for the software package is consistently checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes from the various data sources, to check for the latest updates within a certain period e.g. the past 6-12 months (this month range is used as the ISO usually publishes their updates at the end of the year with occasional mid-year updates). The app compares the generated output with that of the updates JSON currently in the software package and will replace this json to integrate the latest updates found, such that the API will have the most **up-to-date** and **accurate** data. A Cloud Scheduler is used to call the application on the aforementioned schedule. 
 
 Additionally, a GitHub Issue in the custom-built [`iso3166-updates`](https://github.com/amckenna41/iso3166-updates), [`iso3166-2`](https://github.com/amckenna41/iso3166-2) and [`iso3166-flag-icons`](https://github.com/amckenna41/iso3166-flag-icons) repositories will be automatically created that formats and tabulates all updates/changes that need to be implemented into the JSONs on the aforementioned repos.
 
-Ultimately, this Cloud Run microservice ensures that the software and associated APIs are up-to-date with the most latest, accurate and reliable ISO 3166-2 information for all countries/territories/subdivisions etc.
+Ultimately, this Cloud Run microservice ensures that the software and associated APIs are up-to-date with the **most latest, accurate** and **reliable** ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
 * [python][python] >= 3.8
 * [iso3166][iso3166] >= 2.1.1 
+* [python-dateutil][python-dateutil] >= 2.9.0
 
 Installation
 ------------
 Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-updates --upgrade
@@ -193,25 +196,25 @@
 ```
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY:**
 ```python
 iso["BA","DE","FRA","HUN","600"]
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2003 and 2004:**
+**Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2005 and 2009:**
 ```python
-iso.year("2002, 2003, 2004")
+iso.year("2002, 2005, 2009")
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016:**
+**Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016, inclusive:**
 ```python
 iso.year("2013-2016")
 ```
 
-**Get all listed ISO 3166 changes/updates for all countries, for all years after 2017 inclusive:**
+**Get all listed ISO 3166 changes/updates for all countries, for all years after 2017, inclusive:**
 ```python
 iso.year(">2017")
 ```
 
 **Get any listed ISO 3166 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
 iso.year("2012-2021").IE
@@ -279,23 +282,23 @@
   # -verbose VERBOSE, --verbose VERBOSE
   #                       Set to 1 to print out progress of updates function, 0 will not print progress (default=True).
   # -use_selenium USE_SELENIUM, --use_selenium USE_SELENIUM
   #                       Gather all data for each country from its official page on the ISO website which 
   #                       requires Python Selenium and Chromedriver. If False then just use country data
   #                       from its wiki page (default=True).
 ```
-**Get all the latest updates for all ISO 3166 countries**
+<!-- **Get all the latest updates for all ISO 3166 countries:**
 ```bash
 ./get_all_updates.sh 
 
 '''
---export_filename     Filename for exported JSON/CSV files containing updates data (default="iso3166-updates.json").
+--export_filename     Filename for exported JSON/CSV files containing updates data (default="iso3166-updates").
 --export_folder       Folder name to store exported JSON/CSV files containing updates data (default="test-iso3166-updates).
 '''
-```
+``` -->
 
 <!-- **Import module:**
 ```python
 import get_all_iso3166_updates as iso3166_updates
 ```
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
@@ -325,74 +328,84 @@
 **Get any listed ISO 3166 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ``` -->
 
 The output files from the <i>get_all_iso3166_updates.py</i> script for the updates/changes to an ISO 3166-2 country returns 4 columns: 
-<b>Edition/Newsletter, Date Issued, Code/Subdivision Change</b> and <b>Description of Change.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+<b>Code/Subdivision Change, Description of Change, Date Issued</b> and <b>Edition/Newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
-* Date Issued: date that the change was communicated.
 * Code/Subdivision Change: overall summary of change/update made.
 * Description of Change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Date Issued: date that the change was communicated.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
 
 E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
-| Edition/Newsletter | Date Issued | Code/Subdivision Change | Description of Change |   
+| Code/Subdivision Change | Description of Change | Date Issued | Edition/Newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
-| Newsletter I-8.    | 2007-04-17  | Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements.                 | 
-| Online Browsing Platform (OBP). | 2014-11-03 | | Update List Source |
-| Online Browsing Platform (OBP). | 2015-11-27 | | Update List Source | 
+| Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements. | 2007-04-17 | Newsletter I-8. | 
+| Update List Source. |  | 2014-11-03 | Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AD) | 
+| Update List Source. |  | 2015-11-27 | Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AD) | 
 
 E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   "AD": [
       {
-          "Date Issued": "2015-11-27",
-          "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD).",
           "Code/Subdivision Change": "Update List Source.",
-          "Description of Change": ""
+          "Description of Change": "",
+          "Date Issued": "2015-11-27",
+          "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)."
       },
       {
-          "Date Issued": "2014-11-03",
-          "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD).",
           "Code/Subdivision Change": "Update List Source.",
-          "Description of Change": ""
+          "Description of Change": "",
+          "Date Issued": "2014-11-03",
+          "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)."
       },
       {
-          "Date Issued": "2007-04-17",
-          "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf).",
           "Code/Subdivision Change": "Subdivisions added: 7 parishes.",
-          "Description of Change": "Addition of the administrative subdivisions and of their code elements."
+          "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
+          "Date Issued": "2007-04-17",
+          "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
+
       }
   ]
 }
 ```
 
 Directories 
 -----------
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Run microservice for the check-for-updates function which is a periodically called Cloud Run app that uses the Python software to check for the latest updates for all ISO 3166 countries, ensuring the API and jsons are reliable, accurate and up-to-date.
 * `/docs` - documentation for `iso3166-updates`, available on [readthedocs](https://iso3166-updates.readthedocs.io/en/latest/).
 * `/tests` - unit and integration tests for `iso3166-updates` software and API.
 * `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
-* `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium. 
+<!-- * `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium.  -->
 * `UPDATES.md` - log of all the latest updates from 2022 onwards. 
 
 Issues
 ------
 Any issues, errors/bugs or enhancements can be raised via the [Issues][Issues] tab in the repository.
 
 Contact 
 -------
 If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
 <!-- [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/) -->
 
+Other ISO 3166 repositories
+---------------------------
+Below are some of my other custom-built repositories that relate to the ISO 3166 standard.
+
+* [iso3166-updates-api](https://github.com/amckenna41/iso3166-updates-api): frontend API for iso3166-updates.
+* [iso3166-2](https://github.com/amckenna41/iso3166-2): a lightweight custom-built Python package, and accompanying API, that can be used to access all of the world's ISO 3166-2 subdivision data. A plethora of data attributes are available per country and subdivision including: name, local name, code, parent code, type, lat/longitude and flag. Currently, the package and API supports data from 250 countries/territories, according to the ISO 3166-1 standard.
+* [iso3166-2-api](https://github.com/amckenna41/iso3166-2-api): frontend API for iso3166-2.
+* [iso3166-flag-icons](https://github.com/amckenna41/iso3166-flag-icons): a comprehensive library of over 3500 country and regional flags from the ISO 3166-1 and ISO 3166-2 standards.
+
 References
 ----------
 \[1\]: ISO 3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
 \[2\]: ISO 3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
 \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
 \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
 \[5\]: ISO 3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
@@ -406,24 +419,25 @@
 
 [demo_iso3166_updates]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [demo_get_all_iso3166_updates]: https://colab.research.google.com/drive/161aclDjGkWQJhis7KxBO1e6H_ghQOPRG?usp=sharing
 [api]: https://www.iso3166-updates.com/api
 [medium]: https://medium.com/@ajmckenna69/iso3166-updates-d06b817af3a7
 [python]: https://www.python.org/downloads/release/python-360/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
+[python-dateutil]: https://pypi.org/project/python-dateutil/
 [pandas]: https://pandas.pydata.org/
 [tqdm]: https://github.com/tqdm/tqdm
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [google-auth]: https://cloud.google.com/python/docs/reference
 [google-cloud-storage]: https://cloud.google.com/python/docs/reference
 [google-api-python-client]: https://cloud.google.com/python/docs/reference
 [flask]: https://flask.palletsprojects.com/en/2.3.x/
 [emoji-country-flag]: https://pypi.org/project/emoji-country-flag/
 [gunicorn]: https://pypi.org/project/gunicorn/
 [selenium]: https://selenium-python.readthedocs.io/index.html
 [webdriver-manager]: https://pypi.org/project/webdriver-manager/
 [lxml]: https://lxml.de/
-[updates_md]: https://github.com/amckenna41/iso3166-updates/blob/main/UPDATES.md
+[updates_md]: https://github.com/amckenna41/iso3166-updates/blob/main/UPDATES.MD
 [iso3166]: https://github.com/deactivated/python-iso3166
 [PyPi]: https://pypi.org/project/iso3166-updates/
 [Issues]: https://github.com/amckenna41/iso3166-updates/issues
```

