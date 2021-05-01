---
layout: default
title: Toxic Release
parent: The Data
nav_order: 1
---

# Typography
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Notebook

* data.ipynb <br> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vetiveria/spots/blob/develop/data.ipynb)

<br>

## Releases

**Important**: The toxic releases data encoded by [TRI_RELEASE_QTY](https://enviro.epa.gov/enviro/ef_metadata_html.ef_metadata_table?p_table_name=tri_release_qty&p_topic=tri) are the **total on-site disposal or other releases** data values.  In a nutshell, it is comparable with the on-site totals w.r.t. [EPA TRI Explorer Release Facility](https://enviro.epa.gov/triexplorer/tri_release.facility).  For example the

* 'Total On-site Disposal or Other Releases' field of [St. John Baptist Parish (2018)](https://enviro.epa.gov/triexplorer/release_fac?p_view=COFA&trilib=TRIQ1&sort=_VIEW_&sort_fmt=1&state=22&county=22095&chemical=All+chemicals&industry=ALL&year=2018&tab_rpt=1&fld=TRIID&fld=LNGLAT&fld=RELLBY&fld=TSFDSP)

wherein

* state = 22
* county = 22095
* year = 2018

is equivalent to the totals per (REPORTING_YEAR, TRI_FACILITY_ID, TRI_CHEM_ID) encoded by URL

* [tri_facility, tri_reporting_form, tri_release_qty model](https://data.epa.gov/efservice/TRI_FACILITY/STATE_ABBR/LA/STATE_COUNTY_FIPS_CODE/22095/TRI_REPORTING_FORM/REPORTING_YEAR/2018/TRI_RELEASE_QTY/CSV)

built via model

* https://www.epa.gov/enviro/tri-reported-chemical-information-subject-area-model
