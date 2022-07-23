---
layout: default
title: About Geographic Values
parent: The Data
nav_order: 2
custom_js:
- latex
---

# About Geographic Values
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

<br>

## Missing Values

The hazardous waste data sets are w.r.t. facilities in the states and territories of the U.S.A.  The locations of these facilities are encoded by the `fac_latitude` & `fac_longitude` fields.  However, a number of facilities do not have `fac_latitude` & `fac_longitude` values.  Hence, the latitude & longitude values of such facilities are determined via [geopy](https://geopy.readthedocs.io/en/stable/#module-geopy.geocoders).  

<br>
<br>

## Decimals

Each EPA [fac_latitude](https://enviro.epa.gov/enviro/EF_METADATA_HTML.tri_page?p_column_name=FAC_LATITUDE) & [fac_longitude](https://enviro.epa.gov/enviro/EF_METADATA_HTML.tri_page?p_column_name=FAC_LONGITUDE) value is a ***degrees, minutes, seconds*** value; format DDMMSS.  The values are converted to decimal form via the formula

$$DD + \frac{MM}{60} + \frac{SS}{3600}$$

which converts DDMMSS co&ouml;rdinates to decimal form.

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
